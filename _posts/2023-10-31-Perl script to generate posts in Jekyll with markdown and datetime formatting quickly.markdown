---
date: 2023-10-31 15:03:07 +0530
layout: post
title: Perl script to generate posts in Jekyll with markdown and datetime formatting quickly
---
```
#!/usr/bin/perl
use YAML::Dumper;
use DateTime;
my $dt = DateTime->now;
$dt->set_time_zone( 'Asia/Kolkata' );
$h{"layout"} = "post";
$h{"date"} = $dt->strftime("%F %T %z");
print "Enter post title\n";
my $title = <STDIN>;
chomp $title;
$h{"title"} = $title;
print "Enter content\n";
my @body;
while (my $line = <STDIN>) {
        last if $line =~ /nof/;
        push @body, $line;
}
#chomp $body;
my $yaml = YAML::Dumper->new->dump(\%h);
my $ymd = $dt->ymd;
open F, '>', "_posts/$ymd-$h{'title'}.markdown";
print F $yaml . "---\n";
print F @body;
close F;
```


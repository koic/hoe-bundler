# hoe-bundler

* http://github.com/flavorjones/hoe-bundler

## DESCRIPTION:

Generate a Gemfile based on a Hoe spec's declared dependencies.

## FEATURES/PROBLEMS:

Creates a rake task to generate a bundler Gemfile based on your declared hoe dependencies.

* `bundler:gemfile`

Why would you want to do this? I mean, why would anyone want to use bundler to test their gem?

1. to make sure you've declared all your dependencies in your Hoe.spec.
2. to make sure you're testing against the exact versions of dependencies that you're claiming in your Hoe.spec.

## SYNOPSIS:

Just add the following line to your Rakefile before you call `Hoe.spec`:

    Hoe.plugin :bundler

And then run the following command to generate a Gemfile:

    rake bundler:gemfile

## REQUIREMENTS:

* hoe >= 2.2.0

## INSTALL:

* gem install hoe-bundler

## DEVELOPERS:

After checking out the source, run:

  $ rake newb

This task will install any missing dependencies, run the tests/specs,
and generate the RDoc.

## LICENSE:

(The MIT License)

Copyright (c) 2010 Mike Dalessio

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

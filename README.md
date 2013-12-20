# gf-bench

Simpe benchmark tool for GrowthForecast

## Installation

execute:

    $ bundle

## Usage

    $ bundle exec gf-bench http://localhost:5125/ [options]
        -n, --number                 Number of requests to perform
        -c, --concurrency            Number of multiple requests to make
        -s, --skip_initial_post      Do not initial post
        -v, --verbose                Verbose output
        -h, --help                   Display this help message.

## Output Example

    $ bundle exec bin/gf-bench  http://127.0.0.1:5125  -s -c 8 -n 10000
    requests = 10000
    concurrency = 8
    target = http://127.0.0.1:5125


    Benchmark is starting
    processing 0
    processing 1000
    processing 2000
    processing 3000
    processing 4000
    processing 5000
    processing 6000
    processing 7000
    processing 8000
    processing 9000
    req/sec = 574.5350331067195

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

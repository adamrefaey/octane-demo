# Laravel Octane demo

### Demo app running on Octane server with Swoole using Sail

## Requirements

Docker and Docker Compose.

## Installation

```bash
docker run --rm \
	-v $(pwd):/opt \
	-w /opt \
    laravelsail/php80-composer:latest \
    bash -c “composer install”
```

```bash
./vendor/bin/sail build --no-cache
```

## Usage

```bash
./vendor/bin/sail up -d
```

-   After the containers are up, Octane server will run automatically in `watch mode` so you can code and see that reflect in the browser.
-   Octane server will run on port `8000`, so you can open your browser to `http://localhost:8000`

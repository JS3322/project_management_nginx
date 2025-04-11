# Basic Nginx Setup Example

This is a basic Nginx setup demonstrating common configuration patterns and best practices.

## Directory Structure

```
nginx/
├── conf/
│   └── nginx.conf    # Main configuration file
├── html/
│   ├── index.html    # Default welcome page
│   └── 50x.html      # Error page
└── logs/
    ├── access.log    # Access logs will be written here
    └── error.log     # Error logs will be written here
```

## Configuration Features

The `nginx.conf` includes:
- Basic HTTP server setup
- Static file serving
- Gzip compression
- Error page handling
- Example of static file caching
- Commented example of reverse proxy setup

## How to Use

1. Install Nginx on your system
2. Copy these configuration files to your Nginx installation
3. Adjust paths in nginx.conf if needed
4. Test the configuration: `nginx -t`
5. Start Nginx: `nginx`
6. Visit http://localhost to see the welcome page

## Common Commands

- Start Nginx: `nginx`
- Stop Nginx: `nginx -s stop`
- Reload configuration: `nginx -s reload`
- Test configuration: `nginx -t`

## Notes

- The default port is set to 80
- Logs are stored in the logs directory
- Static files are served from the html directory
- A basic caching strategy is implemented for static files 
# Docker FROM Complete

A VS Code extension that provides intelligent autocomplete suggestions for Docker base images when editing Dockerfiles. Get suggestions directly from DockerHub with rich hover information, sorted by popularity just like the DockerHub website.

## Features

🔍 **Smart Image Search**: Type `FROM ub` and get suggestions like `ubuntu`, `ubuntu/apache2`, etc.

⭐ **Popularity Sorting**: Results are sorted just like DockerHub - official images first, then by star count

🏷️ **Tag Completion**: Type `FROM python:` to see available tags for any image

📋 **Rich Hover Information**: Hover over any image name to see:

- Description and maintainer information
- Star count and pull statistics
- Last updated date
- Official image status

⚡ **Performance Optimized**: Built-in caching and request debouncing for fast responses

## Usage

1. Open any Dockerfile or create a new file with `.dockerfile` extension
2. Start typing a FROM statement:
   ```dockerfile
   FROM ub
   ```
3. See autocomplete suggestions appear with DockerHub search results
4. For tags, add a colon:
   ```dockerfile
   FROM python:
   ```
5. Hover over any image name to see detailed information

## Examples

**Image Search:**

```dockerfile
FROM ub        
FROM node      
FROM python    
```

**Tag Completion:**

```dockerfile
FROM python:   
FROM node:     
```

## Requirements

- VS Code 1.100.0 or higher
- Internet connection for DockerHub API access

## Installation

Install from the VS Code marketplace or run:

```
ext install docker-from-complete
```

## Extension Settings

This extension works out of the box with no configuration required.

## Known Issues

- Requires internet connection to fetch DockerHub data
- Rate limits may apply for very frequent requests (cached for 5 minutes)

## Release Notes

### 0.0.1

Initial release featuring:

- DockerHub image search integration
- Tag completion for specific images
- Rich hover information with image details
- Popularity-based sorting
- Performance optimizations with caching

## Contributing

Found a bug or have a feature request? Please open an issue on GitHub.

## License

MIT License - see LICENSE file for details.

---

**Enjoy building your Docker images with intelligent autocomplete!**

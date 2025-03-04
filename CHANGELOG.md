# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [0.1.0] - 2025-03-01

### Added
- Inverted index implementation for faster search
  - Preliminary search using inverted index
  - Fallback to detailed scoring for better results
- Enhanced API functionality
  - Renamed `searchIconsByCategory` to `findIconsByCategory` for consistency
  - Increased result limit from 3 to 5 icons
  - Improved result scoring and ranking
- Project structure reorganization
  - Better organization of domain models and services
  - Improved type definitions for icons and search
- Documentation improvements
  - Updated project structure documentation
  - Added detailed setup and deployment instructions
  - Synchronized English and Chinese documentation

### Changed
- Search algorithm improvements
  - Two-tier search strategy implementation
  - Better handling of Chinese text input
  - Improved category relevance calculation
- Performance enhancements
  - Optimized search index building
  - Improved caching strategy
  - Better memory usage

### Fixed
- Fixed inconsistent API naming
- Corrected project structure documentation
- Improved error handling in search services


## 0.0.1 - 2025-02-27

### Added
- Initial project setup and configuration
  - TypeScript and Cloudflare Workers environment setup
  - Development tooling (Vitest, Wrangler)
  - Project documentation (README in English and Chinese)
- Core API endpoints implementation
  - `findIcons`: Smart icon search with natural language support
  - `getIconCategories`: Category listing functionality
  - `searchIconsByCategory`: Category-based icon search
- Advanced search algorithms integration
  - Jaccard Similarity matching
  - N-gram matching algorithm
  - Category-based matching
  - Exact matching support
  - Levenshtein Distance calculation
  - Name-based matching
  - Tag-based search functionality
- Performance optimizations
  - LRU caching implementation (2000 entries)
  - Similarity threshold configuration (0.08)
  - Multi-language support optimization
  - English and Chinese text processing

[0.1.0]: https://github.com/fradser/mcp-server-remix-icon/compare/v0.0.1...v0.1.0
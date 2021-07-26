# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.6.1]
Fixed
- Check node is present before remove
## [0.6.0]
Changed
- Diagram changes are animated
## [0.5.6]
Fixed
- Fixed an issue where an undefined parameter may be iterated on
Changed
- Use dependency `@appland/models` version `0.6.0`
- Now building sourcemaps

## [0.5.5]
Fixed
- Disable auto-expanding small packages on small graphs
Changed
- Use dependency `@appland/models` version `0.4.0`

## [0.5.4]
Changed
- Backward cyclical references are no longer enumerable

## [0.5.3]
Fixed
- Force zoom-in Component diagram after rendering to make node labels readable

## [0.5.2]
Fixed
- Render border around expanded package on initial graph

## [0.5.1]
Added
- Component diagram edges are clickable

## [0.5.0]
Added
- Add `Models.ClassMap`

## [0.4.2]
Added
- Component diagram "collapsed" node indicates how many nodes it will expand to
Changed
- Edit node colors in Component diagram
- Make container box always visible for expanded nodes
- Component diagram "collapsed" node indicates how many nodes it will expand to

## [0.4.1]
Added
- Add `scrollTo` method to Component Diagram

## [0.4.0]
Breaking changes
- Rename project to `@appland/diagrams`.
- Change models dependency to `@appland/models`.

## [0.3.1]
Fixed
- When there is an active focus, single-click elsewhere on the diagram should not clear the focus
- When highlight is called with a non-null arg, the component diagram should not emit highlight with null before highlight with the non-null arg
- "focus" event is emitted with a null argument when the focus is cleared

## [0.3.0]
Breaking changes
- Component diagram `highlight` event listener recieves array of nodes (in `0.2.*` it recieves one node)
Added
- Component diagram `highlight` method can accept an array of nodes

## [0.2.11]
Changed
- Use NPM package '@applandinc/appmap-models' instead of git package

## [0.2.10]
Fixed
- Fix issue with removing node which contains one child with the same name as parent
- Prevent expanding node which contains one child with the same name as parent

## [0.2.9]
Fixed
- Don't clear node highlight when diagram expands/collapses
- Fix arrows `marker-end` location after expanding/collapsing

## [0.2.8]
Added
- Emit 'focus', 'expand' and 'collapse' events of Component Diagram

## [0.2.7]
Fixed
- Check node has subclasses before expanding

## [0.2.6]
Changed
- Component diagram: expand package which contains only one node by default

## [0.2.5]
Fixed
- Fix `marker-end` location: set local url by hash (`url(#arrowhead1)`) without page URL and query params

## [0.2.4]
Fixed
- Emit 'highlight' event of Component Diagram when node is highlighted

## [0.2.3]
Fixed
- Diagram freezes when panning with `momentum`

## [0.2.2]
Changed
- Component diagram: inbound and outbound arrows now have separate styling
- Component diagram: HTTP child nodes now have separate styling

## [0.2.1]
Fixed
- Potential null reference when highlighting a node

## [0.2.0]
Added
- Context menu component
- The component diagram now displays a frame around classes in an expanded package
- Light and dark themes for flow view and timeline

Fixed
- Component diagram sizing when viewing a small number of nodes
- Fixed visible overflow for large SQL queries in the flow view

Changed
- The default positioning of a component diagram now fills the viewport


## [0.1.6]
### Changed
- Extracted models to https://github.com/applandinc/appmap-models

## [0.1.5]
### Added
- Initial release

[0.1.6]: https://github.com/applandinc/d3-appmap/compare/tag/v0.1.5...v0.1.6
[0.1.5]: https://github.com/applandinc/d3-appmap/releases/tag/v0.1.5

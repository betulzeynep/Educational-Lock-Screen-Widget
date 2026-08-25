# Educational Lock Screen Widget — iOS Prototype

A small iOS prototype demonstrating an educational concept app centered around an iPhone Lock Screen widget.

## Demo

[Watch the demo video](YOUR_VIDEO_LINK)

## What it demonstrates

- SwiftUI companion app
- WidgetKit Lock Screen widget
- `accessoryRectangular` widget
- Timeline-based concept rotation
- Deep linking from the Lock Screen widget to a specific concept
- Local JSON content
- Saved concepts
- Recently viewed concepts
- Lightweight local persistence
- Separation between the data layer and SwiftUI presentation layer

## Architecture

The prototype keeps the content/data layer separate from the presentation layer.

```text
App
├── Models
├── Data
│   ├── ConceptRepository
│   └── LocalConceptRepository
├── Features
│   ├── Home
│   ├── ConceptDetail
│   ├── Recent
│   └── Saved
└── Widget
    ├── ConceptWidget
    ├── ConceptTimelineProvider
    └── WidgetEntry

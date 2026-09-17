# Liberty Hill ISD Boundary Locator

An interactive attendance boundary and campus locator for Liberty Hill
ISD.

The application allows families, staff and district leaders to explore
current attendance boundaries, search for an address, use their current
location, identify assigned campuses and browse Liberty Hill ISD schools
on an interactive map.

## Current Version

**v1.09**\
Released September 17, 2026

## Features

-   Interactive Liberty Hill ISD attendance boundary map
-   Elementary, middle and high school boundary filters
-   Address search
-   Current location lookup
-   Direct map-click assignment lookup
-   Campus directory with search and level filters
-   Interactive campus markers
-   Smooth campus recentering and zoom
-   Selected-campus marker highlighting
-   Assignment results for selected locations
-   Satellite and street map layers
-   Planning notes and map annotations
-   Responsive desktop and mobile interface
-   Mobile navigation drawer
-   Print-friendly styling
-   Embedded Liberty Hill ISD Texas favicon
-   Accessibility and reduced-motion support

## Changelog

### v1.09

**Stability and QA**

-   Fixed a JavaScript syntax error introduced in v1.08 that prevented
    the application from initializing correctly.
-   Repaired the `showAssignments()` function.
-   Prevented the My Location workflow from triggering competing map
    animations.
-   Preserved the closer zoom level for current-location results.
-   Added JavaScript parser validation to the QA process.
-   Revalidated campus selection, assignment lookup, mobile navigation,
    map controls and existing interface behavior.

### v1.08

**My Location Improvements**

-   Updated My Location to smoothly recenter the map on the user's
    position.
-   Increased My Location zoom to level 16 for a closer view than
    standard campus selection.
-   Added a smooth animated transition when locating the user.
-   Added reduced-motion handling for the location animation.

> v1.08 contained a JavaScript regression that was corrected in v1.09.

### v1.07

**Spacing and UI Refinements**

-   Standardized padding and spacing throughout the application.
-   Improved planning-note popup spacing and close-control clearance.
-   Refined campus and assignment popup padding.
-   Improved sidebar, campus-card, address-form and assignment-result
    spacing.
-   Improved Layers and Notes panel spacing.
-   Increased touch-target consistency.
-   Added mobile-specific spacing adjustments.

### v1.06

**Campus Selection and Interaction Polish**

-   Added a persistent visual state for the selected campus marker.
-   Selected campus markers now enlarge slightly and display a gold
    highlight.
-   Campus highlighting clears when another location or campus is
    selected.
-   Added reduced-motion support for marker transitions.
-   Added Escape-key handling for transient interface elements.

### v1.05

**Map Navigation Improvements**

-   Campus selections now smoothly recenter and zoom the map.
-   Campus information opens after map movement completes.
-   Prevented popup auto-panning from moving the selected campus away
    from center.
-   Unified campus-marker and Browse Campuses selection behavior.
-   Removed the redundant Select on Map button.
-   Clicking directly on the map now performs an attendance assignment
    lookup.
-   Preserved map-note placement as a separate interaction mode.
-   Improved mobile campus selection behavior.

### v1.04

**Responsive Layout Improvements**

-   Increased the desktop sidebar width for readability.
-   Adjusted intermediate desktop/tablet sidebar sizing.
-   Fixed vertical scrolling in the mobile navigation drawer.
-   Removed nested scrolling from Browse Campuses on mobile.
-   Embedded the Texas favicon directly into the HTML file.

### v1.03

**Map Cleanup and Branding**

-   Added the Liberty Hill ISD Texas seal as the application favicon.
-   Removed floating school names from attendance boundary polygons.
-   Removed the Boundary Labels control and obsolete label code.
-   Retained clickable attendance boundaries without persistent floating
    labels.

### v1.02

**Boundary and Campus Locator Enhancements**

-   Added attendance boundary filtering by school level.
-   Consolidated high school grades into a single High School filter.
-   Added address-entry functionality.
-   Improved assignment-result presentation.
-   Added interactive boundary lookup behavior.
-   Improved campus and boundary exploration controls.

### v1.01

**Initial Refinements**

-   Improved map layout and navigation.
-   Refined campus marker behavior.
-   Improved district boundary presentation.
-   Removed unnecessary map-key elements.
-   Improved assignment popup presentation.
-   Corrected campus positioning and map interaction issues.

### v1.00

**Initial Release**

-   Interactive Liberty Hill ISD map
-   Campus locations and markers
-   Attendance boundary visualization
-   Campus browsing
-   Location-based assignment lookup
-   Responsive map interface

## Usage

The application is distributed as a standalone HTML file. No Node.js
server, application server or database is required for the public-facing
locator itself.

To deploy:

1.  Upload the HTML file to the hosting environment.
2.  Serve the file through HTTPS.
3.  Open the application in a modern web browser.

HTTPS is required for browser-based geolocation features such as **My
Location** when deployed publicly.

## Data

Attendance boundary information displayed by this application should
correspond to the school year identified in the interface.

Boundary and campus data should be reviewed whenever Liberty Hill ISD:

-   Opens a new campus
-   Changes attendance boundaries
-   Changes grade configurations
-   Renames a campus
-   Changes a campus address
-   Adopts new attendance zones

The current production build is designed for **2026--27 attendance
assignments**.

## Browser Support

The application is intended for current versions of:

-   Google Chrome
-   Microsoft Edge
-   Safari
-   Mobile Safari
-   Chrome for Android

## Accessibility

The application includes keyboard-accessible controls, semantic form
controls, visible focus states, reduced-motion support, responsive
mobile layouts, touch-friendly controls and status messaging.

## Privacy

The locator performs location and address-based lookups to determine
attendance assignments.

The application should not intentionally store user-entered addresses or
device-location coordinates. Analytics implementations should avoid
transmitting precise addresses or coordinates.

## Maintenance

Before publishing a new release:

1.  Validate JavaScript syntax.
2.  Verify all attendance boundary datasets load successfully.
3.  Test address search.
4.  Test My Location over HTTPS.
5.  Test direct map selection.
6.  Test each attendance boundary level.
7.  Test campus search and campus selection.
8.  Verify campus markers and coordinates.
9.  Test desktop and mobile navigation.
10. Test at common mobile viewport sizes.
11. Verify map popups remain within the usable viewport.
12. Confirm the displayed school year is current.

## Versioning

-   **Major version:** Significant redesign or major functional change
-   **Minor version:** New functionality or meaningful UX improvement
-   **Patch version:** Bug fixes, QA corrections or minor refinements

## Liberty Hill ISD

**Vision:** Building Champions in Academics, Character, and Community.

This tool is intended to make Liberty Hill ISD attendance boundary
information easier for families and community members to explore and
understand.

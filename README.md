# 20243007028 - ResponsiveLayout2

COMPX202 / Y05853 - Mobile Computing and Software Architecture  
Practical 2: Implementing Alternative Responsive Layouts

This Android Studio project extends the LinearLayout interface selected from Practical 1 with Android resource qualifiers. Android automatically chooses the appropriate `activity_main.xml` for the current screen configuration.

## Layout variants

- `app/src/main/res/layout/activity_main.xml` - original Practical 1 portrait layout.
- `app/src/main/res/layout-land/activity_main.xml` - landscape layout that uses two side-by-side panels.
- `app/src/main/res/layout-sw600dp/activity_main.xml` - tablet layout for devices whose smallest width is at least 600dp.

No Java code is needed to select a layout. Android resolves the matching resource at runtime.

## Build and test

1. Open this repository in Android Studio.
2. Sync the Gradle project.
3. Run the app on a phone in portrait orientation.
4. Rotate the phone to landscape and confirm the two-panel layout appears.
5. Run the app on a tablet such as Pixel Tablet, Pixel C, or Nexus 10 and confirm the `sw600dp` layout appears.

The layouts use `match_parent`, `wrap_content`, `0dp`, weights, and `dp`/`sp` units. No hard-coded pixel dimensions are used.

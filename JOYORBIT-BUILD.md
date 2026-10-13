# JoyOrbit development fork

Pinned upstream: 5d58223e58f84afb31d5d14a67438841b981a6fa. JoyOrbit adaptations are mirrored here; the application theme, catalogue and build scripts live in PrecisionDataHQ/joyorbit-app (private during development; corresponding source must be published before release). Run its prepare script to restore the pinned Reprise theme/fonts/sounds and replace the stock non-commercial Grid theme.

Android sessions remain open until the library activity resumes. The Java lifecycle bridge is polled by the native launcher after frontend teardown; this keeps play history tied to the actual session. Mac upstream tests23/23 pass after this change; Android build passes. Runtime acceptance is ongoing.

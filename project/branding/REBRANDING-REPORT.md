# Eman Bakeries rebranding review

Complete Flutter source based on upstream mobo-open-source/mobo_billing commit f99933d065784345c8f93b0dd04e2468c038995a. All 266 uploaded source files matched that commit before edits. The parent repository preserves the uploaded JPG, PDF and PNG. The original source archive remains preserved separately in cloud attachments.

## Official logo

Source: EMAN Bakery _ LOGO(png ) 2.png from emanbakery-admin/mobo-billing-app-assets at f1ee7a8. Untouched copy: branding/original/eman-logo.png. Dimensions 4961 x 3509, aspect ratio 41:29, 848941 bytes, RGBA PNG, alpha 0–255, no embedded ICC profile. SHA-256: 0dde4e2d8f9d1d78516e943e9bf61e4743daf259b0d9f0e0572804ba08e0b1d3. Both in-app logo assets are byte-identical to the source. Its opaque white regions have been preserved alongside its original transparency.

## Palette

Solid artwork pixels measured directly: primary green #0D6937; secondary yellow #FCD920; accent red #EA1C2D; white #FFFFFF. Green drives buttons, navigation selection, forms, charts, headers and brand backgrounds through AppTheme, plus remaining hard-coded brand colour references. Yellow is ColorScheme.secondary with dark onSecondary text; red is light-theme tertiary. Both also remain in the unaltered logo. #E7F0EB is a derived green tint, not an original measured logo colour. Neutral backgrounds #FAFAFA and #FFFFFF, text #212121, dark background #121212 and surface #1E1E1E are retained from the original app. Functional status colours remain unchanged.

## Assets and scope

The original logo was neither cropped nor recoloured. All icon derivatives fit the full artwork with aspect ratio retained, accepting integer-pixel rounding. Android adaptive foreground uses a centred 56% bounding box, with every nontransparent pixel verified inside the 66/108-diameter safe circle. Web maskable artwork uses 60%; legacy/iOS icons use 86% and a white background. iOS store icons are opaque. At small icon sizes the full detailed logo naturally loses legibility; no simplified substitute has been invented. Dimensions, file sizes and alpha ranges are recorded in asset-inventory-after.csv.

Login and app-lock retain their original layout, with modestly widened logo boxes. The existing background geometry and onboarding phone compositions remain. Only magenta pixels were mapped to green; the first onboarding panel's embedded Mobo heading was replaced by the official artwork. The replacement splash is a static logo video, 1080 x 1920, H.264, 3.6 seconds, 60,957 bytes; original splash routing, timing and authentication code remain unchanged. Native splash assets use white backgrounds.

Models, providers and existing tests are byte-unchanged. The only service edit changes feedback subject/footer wording. APIs, email recipients, identifiers, billing, navigation, authentication logic and integrations are unchanged. Facebook, Instagram, LinkedIn and YouTube images are byte-unchanged. Upstream README demo images under assets/git remain historical Mobo screenshots and are not used in the app. Upstream legal notices and acknowledgements are retained.

## Verification and limitations

Passed: source ZIP CRC integrity; exact upstream file comparison before editing; original-logo checksum and in-app copy equality; social-icon preservation; unchanged models/providers/tests; image decoding; XML/plist/storyboard and manifest JSON parsing; git diff whitespace check; scan finds no C03355, C53667, FAE6E8 or Colors.pink in lib, Android resources, web or pubspec.yaml.

Flutter analysis, tests and Android debug build were each attempted in project/ and could not execute (exit 127: flutter command not found). Flutter/Dart are absent from PATH; Android tooling was not found in the inspected standard locations. A request to the official Flutter SDK host storage.googleapis.com was blocked by the network proxy (403). A domain addition was saved to the environment draft, but has not been applied or published. No SDK or dependencies were installed. No APK is supplied. iOS builds also require macOS/Xcode.

No application was launched, so there are no live before/after screenshots and no claims of runtime visual, accessibility or integration verification. The supplied preview files are source artwork and splash frames, not app screenshots. Login/dashboard behaviour, dark-mode contrast, responsive placement, adaptive masking and backend-dependent screens still require device/runtime review. Web scaffolding exists, but web compatibility of native plugins is unverified. Upstream does not supply pubspec.lock or Gradle wrapper executables; these are not fabricated here.

When a Flutter SDK with Dart >=3.8.1 and Android SDK are available, run from this directory: flutter pub get; flutter analyze; flutter test; flutter build apk --debug. Use the original login flow to configure an authorized Odoo test server for authenticated visual verification. Do not put credentials in source or reports.

## Review

Changes are on the GitHub review branch rebrand/eman-bakeries, with the untouched import committed separately. Review branding/changed-files.md and the supplied binary Git patch against the import baseline. No release was published and main was not overwritten. The full project ZIP contains all original source paths plus the branding changes and this review record; it excludes caches and credentials.

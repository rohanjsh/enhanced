# TypeSet

[![style: very good analysis][very_good_analysis_badge]][very_good_analysis_link]
[![pub package][pub_badge]][pub_link]
![coverage][coverage_badge]
![pub points][pub_points_badge]

Whatsapp like text formatting for you!!
This supports the input to be formatted with different formatters.
Text style that will support bold, italic and underline text.

i.e.
1. Bold Text will be wrapped in \*asterisk\*
2. Italic Text will be wrapped in \_underscore\_
3. Underline Text will be wrapped in \~tilde\~
4. Bold, Italic and Underline Text will be wrapped in \*asterisk\* \_underscore\_ \~tilt\~


### Preview
<img width="488" alt="Screenshot 2022-12-13 at 11 56 28" src="https://user-images.githubusercontent.com/35066779/207242541-c8bfd00e-0b81-47ce-9bf3-b280e3d63162.png">



## Installation 💻

**❗ In order to start using typeset you must have the [Flutter SDK][flutter_install_link] installed on your machine.**

Add `typeset` to your `pubspec.yaml`:

```yaml
dependencies:
  typeset: #latest
```

Install it:

```sh
flutter packages get
```

---


Usage

```dart
import 'package:typeset/typeset.dart';

TypeSet(inputText: 'Hello, *World!*');
// returns 'World' with bold text

TypeSet(inputText: 'Hello, _World_!');
// returns 'World' with italic text

TypeSet(inputText: 'Hello, ~World~!');
// returns 'World' with underline text

TypeSet(inputText: '*Hello*, _World_ ~World~!');
// returns 'Hello' with bold text, 'World' with italic text and 'World' with underline text

//TypeSet also has a style property which can be used to style the text
TypeSet(inputText: 'Hello, *World!*', style: TextStyle(color: Colors.red));
// returns 'World' with bold text and red color

//OR

//use the simple extension
'Hello, *World!*'.typeset();
//this also comes with style
'Hello, *World!*'.typeset(style: TextStyle(color: Colors.red,),);

```


## Features and bugs

Please file feature requests and bugs at the [issue tracker][tracker].

[flutter_install_link]: https://docs.flutter.dev/get-started/install
[github_actions_link]: https://docs.github.com/en/actions/learn-github-actions
[logo_black]: https://raw.githubusercontent.com/VGVentures/very_good_brand/main/styles/README/vgv_logo_black.png#gh-light-mode-only
[logo_white]: https://raw.githubusercontent.com/VGVentures/very_good_brand/main/styles/README/vgv_logo_white.png#gh-dark-mode-only
[mason_link]: https://github.com/felangel/mason
[very_good_analysis_badge]: https://img.shields.io/badge/style-very_good_analysis-B22C89.svg
[very_good_analysis_link]: https://pub.dev/packages/very_good_analysis
[very_good_cli_link]: https://pub.dev/packages/very_good_cli
[very_good_coverage_link]: https://github.com/marketplace/actions/very-good-coverage
[very_good_ventures_link]: https://verygood.ventures
[very_good_ventures_link_light]: https://verygood.ventures#gh-light-mode-only
[very_good_ventures_link_dark]: https://verygood.ventures#gh-dark-mode-only
[very_good_workflows_link]: https://github.com/VeryGoodOpenSource/very_good_workflows
[tracker]: https://github.com/rohanjsh/typeset/issues
[pub_badge]: https://img.shields.io/pub/v/typeset.svg
[pub_link]: https://pub.dev/packages/typeset
[coverage_badge]: https://img.shields.io/badge/coverage-100%25-green.svg
[build_badge]: https://img.shields.io/github/workflow/status/rohanjsh/typeset/ci.svg
[pub_points_badge]: https://img.shields.io/pub/points/typeset



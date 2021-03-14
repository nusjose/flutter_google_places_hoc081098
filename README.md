# Updated by [@hoc081098](https://github.com/hoc081098). See [file changes](https://github.com/fluttercommunity/flutter_google_places/compare/master...hoc081098:main)

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhoc081098%2Fflutter_google_places&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

- Migrated to **null-safety**.
- Updated dependencies to latest release.
- Refactoring by using **RxDart** for more power.
- Fixed many issues.
- Applied [pedantic](https://pub.dev/packages/pedantic).
- Refactored example, migrated to Android v2 embedding.

```yaml
flutter_google_places:
  git:
    url: https://github.com/hoc081098/flutter_google_places.git
    ref: main
```

# flutter_google_places
<p align="left">
  <a href="https://pub.dartlang.org/packages/flutter_google_places"><img alt="pub version" src="https://img.shields.io/pub/v/flutter_google_places.svg?style=flat-square"></a>
</p>

Google places autocomplete widgets for flutter.

<div style="text-align: center"><table><tr>
    <td style="text-align: center">
<img src="https://raw.githubusercontent.com/fluttercommunity/flutter_google_places/master/flutter_01.png" height="400">
</td>
<td style="text-align: center">
<img src="https://raw.githubusercontent.com/fluttercommunity/flutter_google_places/master/flutter_02.png" height="400">
</td>
</tr>
</table>
</div>

## Getting Started

For help getting started with Flutter, view our online [documentation](https://flutter.dev/).

```yaml
# pubspec.yaml

dependencies:
  flutter:
    sdk: flutter
  flutter_google_places: <last-version>
```

```dart

const kGoogleApiKey = "API_KEY";

Prediction p = await PlacesAutocomplete.show(
                          context: context,
                          apiKey: kGoogleApiKey,
                          mode: Mode.overlay, // Mode.fullscreen
                          language: "fr",
                          components: [new Component(Component.country, "fr")]);

```

The library use [google_maps_webservice](https://github.com/lejard-h/google_maps_webservice) library which directly refer to the official [documentation](https://developers.google.com/maps/web-services/) for google maps web service. 

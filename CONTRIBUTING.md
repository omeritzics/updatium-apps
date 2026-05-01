<div align="center">

[Deutsch](#beitragen)

</div>

# Contributing

- To contribute content, create a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) with valid changes/additions to any files in the repo.
- To test locally, run: `node buildData.js && python -m http.server 8080`


## Contributing Apps

> [!IMPORTANT]
> Please make sure to read the [app criteria](APP_CRITERIA.md) before opening a PR with new/updated app configs.

- You can auto-generate config files from an Updatium export by running `node generateFromExport.js <path to Updatium export>`
- Note: Auto-generated entries will not have icon, category, or description data. Adding those manually is not required but would result in a better user experience.
- You can also auto-generate config files from an Updatium URL redirection link by running `generate_from_url.py`
- Note: Using `generate_from_url.py` requires you to install "Colorama" by using the `pip` command `pip install colorama`


### Minimal Example

To add an app config to this repo, your app configuration JSON must contain at least the `id`, `url`, `author`, `name`, and `additionalSettings` keys. Note that for any app-specific setting you don't define in `additionalSettings`, the default value will be used.

For example:
- Minimal app JSON: `{"id":"dev.patrickgold.florisboard.beta","url":"https://github.com/florisboard/florisboard","author":"florisboard","name":"FlorisBoard Beta","additionalSettings":"{\"includePrereleases\":true}"}`
- As URL: http://http://omeritzics.github.io/updatium-apps/redirect.html?r=updatium://app/%7B%22id%22%3A%22dev.patrickgold.florisboard.beta%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2Fflorisboard%2Fflorisboard%22%2C%22author%22%3A%22florisboard%22%2C%22name%22%3A%22FlorisBoard%20Beta%22%2C%22additionalSettings%22%3A%22%7B%5C%22includePrereleases%5C%22%3Atrue%7D%22%7D

---

# Beitragen

- Um Inhalte beizusteuern, erstellen Sie einen [Pull-Request](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) mit gültigen Änderungen/Ergänzungen zu allen Dateien im Repo.
- Um Ihre Änderungen lokal zu testen, führen Sie bitte `node buildData.js && python -m http.server 8080` aus


## Apps beisteuern

> [!IMPORTANT]
> Bitte stellen Sie sicher, dass Sie die [App-Kriterien](APP_CRITERIA.md) lesen, bevor Sie einen PR mit neuen/aktualisierten App-Konfigurationen eröffnen.

- Sie können Konfigurationsdateien automatisch aus einem Updatium-Export generieren, indem Sie `node generateFromExport.js <Pfad zum Updatium-Export>` ausführen.
- Hinweis: Automatisch generierte Einträge haben keine Symbol-, Kategorie- oder Beschreibungsdaten. Diese manuell hinzuzufügen ist nicht zwingend erforderlich, ist aber erwünscht, weil es zu einer besseren Benutzerfreundlichkeit führen würde.
- Sie können auch automatisch Konfigurationsdateien aus einem Updatium-URL-Umleitungslink generieren, indem Sie `generate_from_url.py` ausführen.
- Hinweis: Die Verwendung von `generate_from_url.py` erfordert die Installation von „Colorama“ mit dem `pip` Befehl `pip install colorama`.


### Minimalbeispiel

Um eine App-Konfiguration zu diesem Repo hinzuzufügen, muss Ihre App-Konfiguration JSON mindestens die Schlüssel `id`, `url`, `author`, `name` und `additionalSettings` enthalten. Beachten Sie, dass für jede app-spezifische Einstellung, die Sie nicht in `additionalSettings` definieren, der Standardwert verwendet wird.

Zum Beispiel:
- Minimale App JSON: `{„id“: „dev.patrickgold.florisboard.beta“, „url“: „https://github.com/florisboard/florisboard“, „author“: „florisboard“, „name“: „FlorisBoard Beta“, „additionalSettings“:„{\“includePrereleases\„:true}“}`
- Als URL: http://http://omeritzics.github.io/updatium-apps/redirect.html?r=updatium://app/%7B%22id%22%3A%22dev.patrickgold.florisboard.beta%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2Fflorisboard%2Fflorisboard%22%2C%22author%22%3A%22florisboard%22%2C%22name%22%3A%22FlorisBoard%20Beta%22%2C%22additionalSettings%22%3A%22%7B%5C%22includePrereleases%5C%22%3Atrue%7D%22%7D

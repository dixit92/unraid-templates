# MangaPixer Unraid templates

Unraid [Community Applications](https://docs.unraid.net/community-applications/) templates for
[MangaPixer](https://github.com/dixit92/mangapixer), a self-hosted, folder-native comic and manga server.

| File | Purpose |
|---|---|
| `templates/mangapixer.xml` | The Docker template for `ghcr.io/dixit92/mangapixer` |
| `ca_profile.xml` | Repository profile shown in Community Applications |
| `icon.png` | Repository and app icon |

## Installing

Search for **MangaPixer** in the Unraid **Apps** tab. Before the listing is live, you can add the template by hand from the
Unraid terminal:

```bash
wget -O /boot/config/plugins/dockerMan/templates-user/my-mangapixer.xml \
  https://raw.githubusercontent.com/dixit92/unraid-templates/main/templates/mangapixer.xml
```

Then **Docker** > **Add Container** and pick **mangapixer** from the Template list. Full instructions:
[Install on Unraid](https://github.com/dixit92/mangapixer/blob/main/docs/install-unraid.md).

## Support

Please open issues on the [MangaPixer repository](https://github.com/dixit92/mangapixer/issues).

## Maintaining this repository

- Keep `TemplateURL` in each template pointed at its own raw URL in this repository.
- After changing a template, run **Validate** and **Scan** at <https://ca.unraid.net/submit>.
- The template tracks the `latest` image tag, so app releases need no change here.

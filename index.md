---
layout: home
---

Compendium of nostr clients and known features.

### Table

<div class="breakout" style="overflow-x:auto;">
<table>
  {% for row in site.data.clients %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
</div>

### Legend

- [NIPs](https://github.com/nostr-protocol/nips)
- ✅ : mostly supported
- 🟡 : partially supported or nonstandard implementation
- ❌ : mostly not supported
- ⚡ : paid feature
- `?` : checked but unclear
- <code>&nbsp;</code> : not yet checked

### Notes

- 🟡 feature may be fully supported on some platforms but not on others (e.g. zaps on iOS)
- 🟡 macOS support for iOS apps that can run on Apple Silicon
- 🟡 mute support (NIP-51) for clients that use kind 30000 parameterized lists instead of the kind 10000 list
- 🟡 reactions support for clients that only allow one kind of character/emoji

### Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>

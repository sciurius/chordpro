---
title: "Directives: key"
description: "Directives: key"
---

# Directives: key

This directive specifies the key the song is written in. Multiple key specifications are possible, each specification is assumed to apply from where it was specified.

Examples:

    {key: C}
    {meta: key C}

Note that if a [capo]({{< relref "Directives-capo" >}}) setting is in effect, the key does not change. This is because guitar players consider the key relative to the chord shapes they play. The actual key as perceived by the listener (sounding key, concert key) *will* be modified according to the capo settings.

For example:

    {key: C}
    {capo: 2}

Now the key for the player is still `C`, but the key for fellow musicians and listeners is `D`.

Metadata item `_key` reflects the key as transposed by the capo value. It cannot be set with a directive but it is automatically provided by ChordPro, and can be used in [title and comment texts]({{< relref "ChordPro-Configuration-Format-Strings" >}}).

See also: [capo]({{< relref "Directives-capo" >}}), [meta]({{< relref "Directives-meta" >}}) and [transpose]({{< relref "Directives-transpose" >}}).

"Watermark" removal "patches" for the album First Love by Hikaru Utada (16 bit / 44.1 kHz)

---

**DISCLAIMER**:
These are not actual tracks from the respective stores,
but "differences" between those tracks,
which are believed to be watermarked,
and the version that is believed to be non-watermarked.
In other words they are meaningful only for someone that already has purchased (or in possession) one of the sets.
It would be extremely wrongful for these to be taken down for DMCA reasons,
especially when this does not need to exist if the Universal Music Group has never come up with such hideous thing
(which deprives people that have purchased the music of what they deserve).

---

NOTE: As you may already know, First Love is the only "old five" studio album by Utada that the original CD master(ing) is not lost from digital stores and streaming platforms,
due to the fact that unlike the other four, its "hi-res remastering" occurred in 2014, before the whole Hikaru Utada catalog was made widely available in 2017,
whereas the "hi-res remastering" occured to the other four one year after that in 2018.
(Also because for whatever reason Universal just decided that they have to "overwrite" the original instead of adding the remasters as new titles.)
Unfortunately I didn't managed to obtain their original CD masters "digitally" (watermarked or not) within that "window".
(I ended up purchasing new Universal Japan reprints for all five of the albums.)

(In addition to that I don't like remasters in general, I despise the 2018 remasters of the other old four because of a couple more other reasons,
so most likely I will never make patches for them. In fact I don't even keep a copy of the version that I believe to be non-watermarked for them.)

The version is that is *known* to be non-watermarked was procured from OTOTOY, which is verified be non-watermarked against a CD rip (of the mentioned purchase / reprint)
using "special techniques" -- you can't just compare the MD5s but would need to "align" their "actual content" first --
not only because optical drives have different "read offsets",
but also because the tracks in the two versions appear to be, for some reason, cut from *vastly* different "track points",
in addition to that they have leading and/or trailing silence of different lengths.
Therefore in some cases you can't even compare track by track but would have to concatenate tracks (or portions of them) and compare the "products" instead.

FWIW, Unlike OTOTOY, AFAIK mora does not have the non-watermarked version of this album (or any of the pre-hi-res Japanese titles by Hikaru Utada),
because the store introduced the "lossless" quality tier (i.e. CD spec/grade files) way more recently.
Anyone who has purchased this album from mora is welcome to share the files with me for me to make patches for them.
(Enough is enough. Not interested in giving more money to Universal myself.)

In addition to OTOTOY, the Tencent stores also seem to have the non-watermarked version of Utada's pre-hi-res catalog.
(You may even find Distance and Deep River on some of them, although I don't think they are "proper" digital releases -- as in, they appear to be CD rips to me.)

---

The MD5s (of the raw PCM samples) of the version that is *known* to be non-watermarked:
```
584926ccb514b7c92c2d8657a1322154
b519f0813649531b725b1a4a910c71fc
041b52c893f06c57cc469dd3503ce8eb
dc98940a551343d9299bdc5469783fe0
e1e6f2eea154232766487d17b73be9c8
d73bd2f4f28298ce79097ea04f703e7d
2c4ffb3f1f4457bd4667c9759c9baa22
20b12a88e1b25d9c9c2947e6d4c67bda
ba7f49077fc1f13113403f6a5ef4cdda
81325b80ee10761ce1bf0500d902548e
ac9992d98474b71a99da63610944139f
ad634b81d2324e0bf0001f889b35498d
```

---

The "patches" were created by "subtracting" the non-watermarked version from the respective watermarked version,
in other words you can obtain the the non-watermarked version by subtracting the corresponding "patches" from the watermarked version you have.
For example:
```
sox -m watermarked.flac -v -1 patch.flac non-watermarked.flac
```
So I suppose you can say that these "patches" are the "watermarks" themselves.

---

The MD5s of the version that is currently available on Qobuz:
```
4e65f6d44e39a5468cd59ed1d5d86d29
963de78f6520287ed2775b243b7d790f
773f83dfa3a22296a4eb3b7b7f3fa953
fb1e77dc384cbc97064952d0f7b9d629
e356c5ae771eaf69a0f684c4c00294b4
3c4df6103ef545c62441aecfca0b63f4
400e8b9edef4698c0adc6d0fbcbe3ce7
c4ae4b42da42a5f5dcea80f4b14e0685
261911729f77053b0e01134a5883abf0
81325b80ee10761ce1bf0500d902548e
839ba3e2d8b6c707bd0d496dc4579991
499a45a8648b12f5cf347a457e1ceff0
```
Patches in `qobuz` are for this version.

---

The MD5s of the version that is currently available on TIDAL:
```
9f237e51fe38f7950192923dce7844fe
a8814d684ece0b2e5f4d22192e1a005b
9aa9b1da98344407ee5e7ed69971d0b4
a5c123de957184cfdabe9557a074dea7
624b010243d178da21793128bc5dbccd
25dbec49a7c759ca649b58a1de3d768a
4f1b38db9a4dc2cd55b045f56e79bc86
35e9e9a95efd19da084891ad0ca07cb6
7225252fbf960eca8961e106b958ead2
81325b80ee10761ce1bf0500d902548e
b0231888a54dc9f0e1de6ad1dec6bf86
dfa143a6a2cb1db974be482ef09994b7
```
Patches in `tidal` are for this version.

---

If you have some other version(s) that you would like me to make patches for (or examine), you are welcomed share them with me. My Gmail is "deumg dot w".
(Better not post a link in an Issue, I think.)

**As mentioned above, the version that I currently believe to be non-watermarked is not leaked from some secret channel, but publicly available for purchase on at
least one digital store.** Also, (for obvious reasons) I myself have made **multiple** purchases of this album.

---

P.S. MD5s of the raw PCM samples can be obtained with `metaflac --show-md5sum`.
If you get all zeroes with that, you can re-encode your FLAC files to have them fixed.

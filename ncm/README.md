The version that is currently on Netease Cloud Music (NCM), of which the MD5s are:

```
58a857425d4a0952892a46852435e14c
b84db1669b4ad74caff7abc56b0a5cc8
385e9b7f74bfb8127bdf6b7147f91ddd
56ac11aa997cfb20a03ceac7b37a32a7
9adcd9bc0b648ad2715b8dab385e9742
57f23f8847193de0a3bb32307e053ee7
a7862880e528dd90fdb2a279879abfda
56bed851156a6b2aa51e8568ec8450a7
ab9ed85198a3b38c1915c8355d6ebf00
16a54b621338f753d611025bde1e6f9f
48b6c6505244e64c255c15204fa517ae
bda9fa936b2671a05fd68a2cec163e5e
```

is confirmed to be non-watermarked. However, unlike the "proper" digital release, it is not a "subset" of what is on the CD I have.
While it miss out less samples / silence than the "proper" digital release does, for some reason it also has some samples (at a non-overlapping position)
that are not found on the CD.

Here is a "graph" that depicts the details:

```
   38190600 {1993} 11371094        94068729 [13035]
() 49561694                 (2002) 94068729 []
```

The two lines represent sample "blocks" in the NCM version and my CD rip respectively:
- `{}` denote that the respective samples that are only found in the NCM version
- `[]` denote that the respective samples are *trailing silence*
- `()` denote that the respective samples are only found in my CD rip
- The numbers are the lengths of the blocks in samples
  - Numbers that are not enclosed refer to samples that can be found in both versions
- Blocks without length specified denote that the exact length of the respective block depends on the read offset of the drive used to make the rip
  - Nevertheless the *total* length of such blocks should be the same with at least *prints of the same pressing*
    - With my CD rip it is 13035 samples
    - In other words, with `{1993}` and `(2002)` removed the two version would be of the same total length

It might be worth mentioning that `{1993}` are the leading samples in the file of track 04.

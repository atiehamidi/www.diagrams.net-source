---
layout: post
author: draw.io
slug: rough-style
date: 2020-06-23 09:24:00
title: Support for hand-drawn diagrams with rough.js
tags: [features, handdrawn]
categories: [features, shapes, connectors]
---

A more relaxed and informal style for shapes, fills and lines is often used in infographics, teaching materials, maps and reports so that the diagrams are little less sterile and boring. The rough style adds a hand drawn shading options, rough outlines and connectors, and handwritten text labels.

We spent a couple of hours integrating [rough.js](https://roughjs.com/) to update our existing, and fairly limited, comic style, and the result is pretty useful.

**Note:** This rough style is available in version 13.3.1 onwards.

## Apply the rough style

1. Select one or more shapes and connectors that you want to roughen.
2. In the format panel on the right, click _Sketch_ to apply the rough style to your selected shapes, labels and connectors.

<img src="/assets/img/blog/sketch-format-panel.png" style="max-width:100%;height:auto;" alt="Select shapes, click Sketch in the format panel, and save your diagram to make it more informal">

### Use the comic style

The rough sketch style appears more like a handdrawn diagram. Use the comic style for a more subtle effect.

1. Select the shapes and connectors you want to apply the comic style to.
2. In the Style tab of the format panel, click on _Properties_.
3. At the bottom, change the _Sketch Style_ dropdown to _Comic_.

<img src="/assets/img/blog/shape-properties-sketch-style-comic.png" style="max-width:100%;height:auto;" alt="Change the sketch style to comic for a more suble handdrawn effect">

### Change properties to customise the sketch style

There are many other properties you can change to customise the sketch style. Note that not all of these properties are applicable to the style you have chosen, but may apply to a different style.

Click on a shape or connector, then expand the _Properties_ section in the _Style_ tab of the format panel on the right. The most common properties are as follows.

* _Jiggle_ - how roughly or randomly the borders, connectors and the fill colours are drawn.
* _Fill Weight_ - set the width of the 'pen' used to draw the fill colour in a shape.
* _Hachure Gap_ - set the distance between the sketched fill lines.
* _Hachure Angle_ - set the direction of the sketched fill lines.
* _Disable Multi Stroke_ - use only one pass of the 'pen' in the sketched border of a shape or a connector.
* _Disable Multi Stroke Fill_ - use only one pass of the 'pen' in the sketched fill colour in a shape.
* _Sketch Style_ - choose between the rough and comic sketch styles.

<img src="/assets/img/blog/sketch-style-properties.png" style="max-width:100%;height:auto;" alt="You can change many style properties to customise the rough and comic sketch styles in draw.io">

## Change the style of the entire diagram

You can set a new global style using one of the presets instead of selecting shapes and connectors and applying styles individually.

1. Make sure nothing in the diagram is selected, then click on the _Style_ tab in the format panel on the right.
2. Select the style settings you want to use. Use the preset styles to change the colours of the shapes, their borders and text, connectors and the drawing canvas. Use the checkboxes to quickly change other style settings:
   * _Sketch_ applies the rough style.
   * _Rounded_ rounds the corners of the shapes.
   * _Curved_ changes the connector style to curved.

<img src="/assets/img/blog/style-tab.gif" style="max-width:100%;height:auto;" alt="Use the styles in the Style tab on the right to change colours and shape and connector styles">

### Use the ``rough=1`` URL parameter

Alternatively, add ``rough=1`` as a URL parameter so the whole diagram has that style. For example, when using the free draw.io online diagram editor:

[```https://app.diagrams.net/?lightbox=1&rough=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fmaster%2Fblog%2Fgitflow-examples.drawio```](https://app.diagrams.net/?lightbox=1&rough=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fmaster%2Fblog%2Fgitflow-examples.drawio)

[<img src="/assets/img/blog/rough-gitflow-example.png" style="max-width:100%;height:auto;" alt="A sketchy gitflow using the rough style">](https://app.diagrams.net/?lightbox=1&rough=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fmaster%2Fblog%2Fgitflow-examples.drawio)

[See a description of all of the supported URL parameters.](/doc/faq/supported-url-parameters.html)

The rough style can make flowcharts a little less intimidating in training and onboarding materials.

<br /><a href="https://app.diagrams.net/?rough=1#R7Vxtc6o4FP41frwdXsTqx2q1d3ftbKftTnf2W4SjZAVCQ6h6f%2F0mEESML%2FhOZ%2Bk4CichQJ4nzzk5gTbMnj9%2Foih0n4kDXsPQnHnDfGwYRts0%2BbcwLFLDvdZMDROKndSk5YY3%2FAtSo55ZY%2BxAJG2piRHiMRwWjTYJArBZwYYoJbNitTHxnIIhRBNQDG828lTrB3aYK2%2FL0nL7T8ATNzuzrskSH2WVpSFykUNmBRPM2YAETF7iC1AfBRAwXvKM6BRow%2Bq7jIk7fWgYA%2F4Zi9p3E0ImHqAQR3c28bnZjniVwRj52BPdvNJQVzbET2f2G2aPEsLSLX%2FeA09AVYRhsKV02Q9UtFvigHDe%2Bfv9H%2Fz5%2B8vo830I3T5ynR%2BylS%2FkxbJ%2FX%2Fqvf3DLXy%2F86%2BO395%2F8h9%2BrNnx4f%2B%2FLfmOLDAzehaHYZGgkTF3bxZ4zRAsSs8ya7XU59EMcJNTRRVXixX6waokYokwSrqlxg8t8T5bNXMzgLUS2KJxxYqcteCiMcHLqR3EABTumEf6CV4jSdoQV5iEKHLkTEhwwoP0vSGEWNgHim7yp9NJ8bMvtMfa8HvEITW7YdBC0x3ZysZRMYaVES%2F5ka4MNyGcUkudLr09vLtvK2GzIs35kLDZFVyDbjSk8iRt%2FtLhBRT%2BDEiiD%2BYpJsuEJiA%2BMLngVWdqRpJdC0JS7s3xUte6lzV0ZUWY2oJAcJpNlyzn7%2BIYk4AFkNBQyKoQDh4uB3CWUuWRCAuT1c2s3tw4JCSWK%2FwJjC9nlKGakSK6j8G7ZbRiNj8KbkjhwwFnS%2Fhzo7xrdEYmpDTvq3UsdR3QCO9uTFQUKOxlGwUOMj8Oi%2Bp%2BbL6bCl14cMd44VYVqhn2PAyM6k1D8iyOCvFVJSK7N6vIPZ3dPu7MaFj%2Bux%2Ff1fJ9%2FRHXKeiTgsCGc9D6giM0gYreUsB0UHo%2FHhq1SOCBJb9xKrXZ6o%2F0SdqBm6e1LaVZT4eAAkoCLYcqH%2BA4eygAJ5dhXkT2OBW2n%2BS3YY5Zmz3wre3Tzquyxagd3EuTNkg6uVdLBVcu%2FtRRteRMKoXCm2N2blGKFC4jaEiprn%2BNo27DBcfCSUdtqWreMdXdKcenxbxQD4JYqB50NatC8lBjcq64Ec9k2tBGimPuGHbhr%2B3G%2FtgZUGGjduDHSbQXpZzQFIVAUBRGyGSZBHTpUOXTQ71UKmdeNPDsKiV7hMxbzEEPj3olBrRdrw%2B3b6kWWe13BuhsvapxPxVm3qga0mo%2BV08kQ6HRR%2B4Qq%2BwTr9vNJvc6YnpiBKpsy1SU99udMZbRakTmlriZNHykOprUz2SbF33U6qaupyX6gZiTr5MF54L597GCpQeKWxEG9GvIdApCDV0OMDRTcuBxyufhDTVkeH7NWhDFbHFclGWOVpsyBSyCXY4ya9XyiAKIH7W2Luf%2FbkKR1KLxrPurmLkpNfNbyUGV5KJ3mvJw%2BqGlOhTL1FPcgFshBuHeKm6nF3iluBklFpriGmi19sG0Iefe3PBGXjmiBP63PWDyDmSDyI1UF8cSj3gznSa9m5XxrIn5DtPATMGu3VFT1o%2FOut%2FZLhpp2%2FaBYJEM0BxjCXnQm6ohlPR7XhKrXkw%2FSOsSOE3LtJdAoZdtwVDNKDXT0coRqXYxQhkIoucK7OcmWwR9SYoN4dnwv%2BsieThLB%2BTNmHg6gJoGR41kVWVFzrXW4W%2BVwt%2FQKzsXCXUNN2tbh7lWegdfLPgTfOXewmxz6QClarFSQadi85RdhWAmh1rWutfb2z5762RpkTtb0CnLqLm%2FlBDarKemazVdhc6fs1E2v1tStRP64JswlCLN8l3PverZ2bsYcpX%2FLt9BK6t96%2Fevon5rcrul8HW9eOnd1djqfJoDtmiDX0TujrN6ZldA7yzxM79brZ48nHKl3fDd%2FUz2tnv93AbP%2FHw%3D%3D" target="_blank"><img src="/assets/img/blog/rough1.png" style="max-width:100%;height:auto;" alt="A flowchart styled by rough.js" ></a>

<br /><a href="https://app.diagrams.net/#R7V1dd6o4F%2F41Xp4uIBDwslU7Z9Y67XRNz5p555JqVN5B4gD2Y379JBCU7ESPegBD294UE9jEnf3szyQO0Gj1%2Bksarpd3dEbigWPNXgdoPHAcO8AW%2B8db3kSL7YqWRRrNyrZaw2P0LxE3Vq2baEYy0VY25ZTGebSWG6c0Scg0l9rCNKUv8m1zGs%2BkhnW4INIweMPjNIyJctuf0Sxflq2Bg3ftX0m0WFZvtvGw7HkKp38vUrpJxPsGDpoXf2X3Kqxoifdmy3BGX2pNaDJAo5TSvLxavY5IzJkrs%2B12T%2B923ClJ8mMecMoHnsN4Q6oR45g9erPmo8vfBEfwPxs%2BpJtVmC6iZICuWa%2B1ZhN%2BU3wr3vglp%2Buyw606cvKafwnjaCGemLJRkbTWNyNTmoZ5RMUNjG8kjaOEFPdUL2VXC%2FG%2FGFqWpzRZVK0PKZ2SLGNP29UNT%2BmAf%2B9b%2BCBrkp%2Btdaxh23IPkdMZE5N5XvYEogd%2Bs8e3LCcrdsNjvmGgOTCqNt7%2BkBImMeU0aF%2FtSC91nkmaRwws1%2BXMjlfRbMb7bsRUj7fzTNmt87gQ8HnEBA%2FdzGmSC7zbjvh8G66imKuKryR%2BJpw0Z3%2B%2BivlN7LLAE5mJTwUFMRhbSMPfW5gifgd71YjGNC2Giyb49nY0Yu1Tuoqm4ikVKAI7%2FMuR11qTAM4vhK5InrLJsUSvg4Q6eAOfX3Yqw6402rKmLoaiLRRaarElvUMquxBg1QMXKcCdJGy2CUkjLt5gxl6WUU4e1%2BGUf35hSls3WXun9WSO3962xHFX5rjtqBwfahiOG2C4qzD81%2BSZZDlNs%2FfK7spoV%2FLt2Z1x21O4%2Fdv9l%2FHk7vp%2BzLXkX4%2FfJ3fsYjz5Y%2FLtt4e7yf13ZRKYaV3zy7WwD%2Bjm56YlK7WWdWW5vnfeNI1GraDCsq6G9T9bmjY0VKfNtTTz5jUwb%2Fg9%2BRNO%2F%2F2J6ySM37Io%2B7Trx%2BMJDWW9Z7sd2nW%2F%2FwD6Aaz2QsdCvcXbtyjLWfcDzbLoiVHu2IHfhQ803vDJ%2B8T7CXjHATCYvmowW8N78IHx7vYW72OShxGfxtGSZmRP1Nwi3gXMP1F%2BPMo9DKIZt0OUDz8wyr3eovyevHCbKoxrtxAfk4zP5yfAjwc4SFd4FZi7AHhF90MiHPcb4Zfx1bt964jFBHm6mX56DacpFTsIrtz9ubVudYxarLsLk3BBVvz7vdMcNAYcx9aVVf9zFP63lZK21ZLL%2B2c%2F8tCVV%2Be3XIDBnir%2FrfFfrcB8gJIXcuXcvi%2FrHwd0dzcbaoXmD5LM3nE1zHOHOl5fAAlIV2UBTCezBanYltDCD0zopNa442WNd8Mhx7jCZedYbmZ0k07FCIS6zJmLQsRdYph8bAc5XremukrVtjElMXN6n4k0CB1rxTseaMR19a5yJs2hUgErv454aDc%2FCh0bELIhoZIJCqFiorff%2B7i51xUIjJt7twdzH4A5gy7asZOPACFIp7m5tyud9RGDTL%2FfQeaF0kiPTPryDaccJrOuX%2F6dZHnhmn3Gm8e7e0iON13Z3%2Bsy3vR06gaammR2zdfbXszSDFVLU6nJH5qan%2FYePBaLBvYQ%2Byw4tG3kSXPlBoDisQbFtawr5PgBDgLm33vBUKaL23MuPDXDwPPQKcMJ15bM7USv1xwMm6TIJDFs5m%2BKTHBbwSeXefwM%2Fd%2B5nRl%2F8XRQbjpZg2VO6RasIQ1YnCbAomYH%2BsS6bTVs6w2pa15aY50a2I%2FpdMPTKtWa5C33UsqXOWQRU%2B4hN%2BHrlP6fTHM16LycEAZyigRp6oytcVINylWNXdPOJH6iLzV1fVM0sI4lTaN%2FmU0M47b1t6fqb9MiBU%2F27z10ZqBgA0IuJLRHkTMDG77VblvzG7IDdglUupEv7QFhFyXFs63EiekHA6TMUaXMM1zKrKakDBJqSspA2Itww1KmJjomcfjEA1BSswhTylfe3T6RhMyjvNZRBKrmmAVkXdAs6BaZmQ1YjVnAhgEW5n0qNXu6vw8IOZBQQ4h1wQIJZDeMWN0qJ7PFDJtvF5DXlJh5HYkZdD%2BcZsWsIl83DK9RlWmq1P9MjiCMMQOBXL%2BWoy5mU6USU4A6sxFYTfbcE56TDTmdnVUlpbgZFHC5gS2x1JFZ6sm9VndxLXYUlj6kdJGWie4dR9c0NSmA9VzvgIgytSbzs0MRVVMsfeAnBmbXdrGOv10wUE209IGBPoAw0JlY29sFO%2FuXbdH4O9WqMmMcHpi%2BsPUm8%2BQyLSALqQKyjfncckq6OgilMWeoqVxMVX%2FjTQl7%2Ff8GfKuz41Wf%2Fxp0UMwJeiCe2%2FTfzy4awYBQi4tG8ImLRgzQVH4PRAGDxaiy54ngUq9jBcM%2FSFZZQdagmPQvT6TRGKYF8J4P4uHgTLnYFv%2F3aZ6GbJYy4IYzu%2FjEPFFGFjySrwta17nHwDCZQjCVd66ugTnBY7XLyTIFl1qKKmlTMlWJ7OGkUHFSnUGRDfMlDhkQ1%2FrB4u62IhtfTQZN%2FtlE63Knw5ad2ZpMoznzGs3KsWHbA3zsLib0nYZMaM0f71rZ%2BYYpu20p9GdLoxgQaqs0imEJtuFCi68mwswWMo0zb5qXBqsWZwsZPGegMyFDDQuZmiz83bzkP64e2R52Bmym253qV9OB23N5akbzevYcsshowblYby%2FWZ1vfolVU1qxMYjKConaplKvfv6VHmgXKxuk%2B4Jx7Z0eogJALCbUUoboNr3Dz%2B5cv0%2FhxQ9PEDPpx5%2B64gg6he%2BSWq5PFDJryoGEx61%2B%2Bze6DnAFz5Z%2FtygFC%2BEhX7hxRUHNiX8N09sJmY1Dt3ao8hUc6z0UHj8BNchQcsFVFs12pLdcgUHMWDYCJvEZ5UQoT17wMZl0V5%2F92vq0JmYYzYO39cxfGQ7cBt7Qw3vX172lKnweOIoKa9RW%2Fm7a%2BAi6gkrccMgxfyNkPmkpzdGge7R7g1gHu054y5qkodtChpY0t7loMjlrWZB7sILDko10g7pzucNe%2FdU2Vn2E07uyDAPHdM63nD3AHyTa1%2FccFZqJpW6pmevoAasfztPnHnRa8lDFtKqXRVc1AC2nXMEgDh%2FJsDNvQMz0StecAq39JB03O4egzHj63b%2BrfA3%2FkoukUatC%2FzWA65920VL0nn0EXgMMGtkvEThe7Q4fbuZBsUwG53a4QVjIuHVKYZvKZEobl0LY7sSqe4O6chOqs1Rq%2FRtzcF2t8eMFyVOdbdaBV1RBHT2mYRiaVh22wtdbF2r1iXbDW6Z0%2B1JldyzB9CGMfW%2Fa3zzfDB4Oq1s5UgMa%2FaX3Yw4yaJgwwzSjv%2B%2BGBk4UOEGrL7DpwPUfTYqYm5B6hsTDM6tpoeChu97B2T2wXdkNNxm1%2FGsRQXrrOwTMML2iD1ZySIpfPlX9oCjeRB84EgMxsi33s4%2B53yEstsPu1dzT5Dw%3D%3D" target="_blank"><img src="/assets/img/blog/rough2.png" style="max-width:100%;height:auto;" alt="A flowchart styled by rough.js" ></a>

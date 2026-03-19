+++
title = 'Static website and layout setup'
date = 2026-03-19T14:40:00+02:00
draft = true
tags = ['website', 'hugo', 'theme']
+++

This is a first post to test out a static website layout using [Hugo](https://gohugo.io/) with the [HugoTeX](https://github.com/kaisugi/HugoTeX) theme and some personal tweaks.
It's published here until I have set everything up the way I want it.

Below there's some lorem ipsum generated text to test sidenotes,
tables, code blocks and more for the theme.

## Layout test with lorem ipsum

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent non mollis
purus. Maecenas rutrum laoreet metus, nec fringilla quam auctor sit amet.
Praesent dignissim justo sit amet est suscipit, vel finibus lectus facilisis.
Aenean volutpat velit velit, nec sagittis elit hendrerit non. Maecenas aliquam,
libero a porttitor viverra, quam libero finibus tellus, id aliquet massa ipsum
nec est. Morbi purus lectus, iaculis id congue et, sollicitudin ut est. Nam ac
nunc et mauris accumsan malesuada vel non ligula. Vivamus semper lectus eget
velit hendrerit cursus.

Praesent elementum metus ac arcu bibendum porta. Quisque metus lectus, eleifend
vehicula lacinia vel, euismod et mauris. Nulla tellus tortor, mollis in tellus
in, suscipit dapibus leo.{{% sidenote %}}Morbi ultrices lacus et tempor laoreet.{{% /sidenote %}} Nam
varius felis ipsum, eget finibus nunc lobortis ac. Fusce nec massa dui. Aenean
ipsum quam, tincidunt et finibus porttitor, pretium sed ante. Quisque bibendum
elit ex, eu porta ex pulvinar eget. Nulla nisi ex, facilisis a magna ut,
tincidunt bibendum risus.

| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | €1600 |
| col 2 is |    centered   |   €12 |
| col 3 is | right-aligned |    €1 |

Fusce sed libero id mauris accumsan suscipit. Maecenas iaculis mollis ante eget
mattis. In ullamcorper lectus vel justo tempor, sed vehicula velit accumsan.
Nulla vitae lacus a magna venenatis sagittis. Sed efficitur ex nibh, quis
rhoncus odio scelerisque eget. Maecenas pharetra lacus eu tortor eleifend, quis
venenatis nunc pharetra.{{% sidenote %}}Pellentesque ac mi non mi convallis euismod.{{% /sidenote %}}
Praesent ac egestas libero, ac lobortis mauris. Fusce nisl est, sollicitudin ut
nisi vel, tincidunt vulputate nibh. Morbi id nibh iaculis, vehicula orci eu,
varius lacus. Maecenas turpis leo, aliquam quis laoreet ac, eleifend nec nulla.

```elixir
pixels = <<213, 45, 132, 64, 76, 32, 76, 0, 0, 234, 32, 15>>

for <<r::8, g::8, b::8 <- pixels>>, do: {r, g, b}
[{213, 45, 132}, {64, 76, 32}, {76, 0, 0}, {234, 32, 15}]
```

Nulla facilisi. Pellentesque mattis est a rhoncus ullamcorper. Nulla scelerisque
sollicitudin justo, a consectetur arcu blandit iaculis. Nunc venenatis tempor
leo, dictum egestas est egestas ac. `for <<r::8, g::8, b::8 <- pixels>>, do: {r, g, b}`
Ut id dui a nulla facilisis fringilla sit amet quis lorem. [Nunc pharetra](/tags/ipsum),
sapien eget interdum venenatis, velit lorem porttitor nisi, quis tempor diam diam 
consectetur justo. Nulla dictum nisi et consequat eleifend. Curabitur consectetur 
nibh quis risus lobortis efficitur. Cras lacus neque, iaculis hendrerit eros non, 
fermentum gravida tortor. Sed finibus aliquet augue et placerat. Ut tincidunt enim 
id rutrum vestibulum.

{{< highlight go "linenos=inline, hl_lines=3 6-8" >}}
package main

import "fmt"

func main() {
    for i := 0; i < 3; i++ {
        fmt.Println("Value of i:", i)
    }
}
{{< /highlight >}}

Suspendisse potenti. Fusce lacus odio, imperdiet sed finibus sed, finibus a
tortor. Fusce finibus, magna in maximus cursus, odio enim sodales diam, at
tincidunt libero ipsum eu eros. Suspendisse molestie malesuada erat ut semper.
Sed eu sapien sit amet leo sagittis varius et non dolor. {{< highlight go "hl_inline=true, style=emacs" >}}fmt.Println("inline"){{< /highlight >}}
Curabitur ac eleifend dui, vel congue nisi.

---
Sed consequat, ligula in pharetra ultricies, nunc ligula
iaculis ipsum, id efficitur lorem nibh ut elit. Praesent vel vulputate sem, nec
ullamcorper felis. Maecenas dui ex, blandit et quam in, venenatis tincidunt ex.

> Curabitur et sapien elit. Maecenas id tortor vitae nibh tristique tempor.
Nulla sed volutpat sapien. Fusce vitae magna nulla. Donec tempus id elit sed 
dictum. Aliquam ac gravida enim, sed aliquet magna. Vivamus sit amet ante 
convallis, congue diam a, sollicitudin urna. Sed imperdiet libero id ornare 
vestibulum. Sed dapibus tellus ac velit maximus, in facilisis metus interdum. 

{{< details summary="See the details" >}}
Etiam aliquam ex lacus, sed ultricies metus ullamcorper ac. Fusce lectus ligula,
vulputate in ultrices ac, pretium eu lacus. Aliquam non ex a diam tincidunt
ullamcorper. **Praesent** pulvinar massa non eros venenatis pharetra. Nam mi nibh,
mollis non tristique eu, ullamcorper id tellus. Quisque sodales nibh ipsum, et
mattis odio hendrerit ut. *Aliquam erat volutpat*. In hac habitasse platea
dictumst. Aenean vitae rutrum ex. ~~Nullam id feugiat ipsum~~. Suspendisse non 
semper risus.
{{< /details >}}

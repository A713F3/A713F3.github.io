---
layout: page
title: QrSnake.ASM
description: Snake game in Assembly that fits in a QR code.
img: assets/img/projects/snake_qr.png
importance: 2
category: fun
related_publications: false
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/snake_qr.png" title="qr" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/snake_gameplay.gif" title="gameplay" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Executable QR and gameplay.
</div>

Snake game in 8086 Assembly for DOS.

Assemble in DOS with MASM.
```
> MASM SNAKE.ASM
> LINK SNAKE.OBJ
> EXE2BIN SNAKE.EXE SNAKE.COM

> SNAKE.COM
```

Qr encode and decode.
```
// Encode
> qrencode -8 -r SNAKE.COM -o snake.png

// Decode
> zbarimg --raw --oneshot -Sbinary snake.png > snake.com
```


<a href="https://github.com/A713F3/QrSnake.ASM" target="_blank">
    <i class="fab fa-github"></i>
    GitHub Repository
</a>


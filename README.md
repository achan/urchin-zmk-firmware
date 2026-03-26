# Urchin ZMK Firmware

Firmware for: [Urchin Keyboard](https://github.com/duckyb/urchin)

## Keymap

34-key layout with homerow mods, ported from Corne-ish Zen.

### Layers

**BASE** - QWERTY with homerow mods
```
╭─────────────────────────────╮ ╭─────────────────────────────╮
│  Q    W    E    R    T      │ │      Y    U    I    O    P  │
│  A    S    D    F    G      │ │      H    J    K    L    '  │
│  Z    X    C    V    B      │ │      N    M    ,    .  CAPS │
╰────────────╮  HYP  SPC/SYM  │ │  NUM  MIR  ╭────────────────╯
             ╰────────────────╯ ╰────────────╯
```
Homerow mods (tap = letter, hold = modifier):
- Left: A=Ctrl, S=Alt, D=Gui, F=Shift
- Right: J=Shift, K=Gui, L=Alt, '=Ctrl

**SYM** - Symbols (hold Space)
```
╭─────────────────────────────╮ ╭─────────────────────────────╮
│       ▽    ^    ?    `      │ │      [    <    =    >    ]  │
│  !    @    #    $    %      │ │      {    (    :    )    }  │
│  \    ~    |    &    ;      │ │      /    *    -    +    _  │
╰────────────╮   ▽      ▽     │ │   ▽    ▽   ╭────────────────╯
             ╰────────────────╯ ╰────────────╯
```

**NUM** - Numbers & Navigation (hold right inner thumb)
```
╭─────────────────────────────╮ ╭─────────────────────────────╮
│       ▽    ▽    ▽    ▽      │ │   PGUP PGDN HOME  END  VOL+ │
│  1    2    3    4    5      │ │      ←    ↓    ↑    →  VOL- │
│  6    7    8    9    0      │ │      ▽    ▽    ▽    ▽  MUTE │
╰────────────╮   ▽      ▽     │ │   ▽    ▽   ╭────────────────╯
             ╰────────────────╯ ╰────────────╯
```

**HYP** - Hyper Keys & Bluetooth (hold left inner thumb)
```
╭─────────────────────────────╮ ╭─────────────────────────────╮
│ H-A  H-G  H-S  H-X  H-F     │ │      ▽    ▽    ▽    ▽    ▽  │
│ H-W  H-C  H-D   ▽    ▽      │ │      ▽    ▽    ▽    ▽    ▽  │
│ CLR  BT0  BT1  BT2  BT3     │ │      ▽    ▽    ▽    ▽    ▽  │
╰────────────╮   ▽    BOOT    │ │ BOOT   ▽   ╭────────────────╯
             ╰────────────────╯ ╰────────────╯
```
H-x = Hyper+key (Ctrl+Alt+Gui+Shift)

**MIR** - Mirror (hold right outer thumb, for one-handed typing)
```
╭─────────────────────────────╮ ╭─────────────────────────────╮
│       ▽    ▽    ▽    ▽      │ │      T    R    E    W    Q  │
│       ▽    ▽    ▽    ▽      │ │      G    F    D    S    A  │
│       ▽    ▽    ▽    ▽      │ │      B    V    C    X    Z  │
╰────────────╮   ▽      ▽     │ │ BSPC   ▽   ╭────────────────╯
             ╰────────────────╯ ╰────────────╯
```

### Combos

| Keys | Output |
|------|--------|
| H + J | `<` |
| K + L | `>` |
| J + K | `:` |
| V + B | Esc |
| F + G | Tab |
| D + F | Backspace |
| N + M | Enter |

## Flashing

1. Download firmware from [Actions](../../actions/workflows/build.yml?query=is%3Asuccess+branch%3Amain)
2. Connect keyboard half via USB
3. Double-tap reset to enter bootloader
4. Copy the `.uf2` file to the mounted drive
5. Repeat for other half

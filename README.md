# How to

1. Commit changes
2. Push to repo
3. Wait until Github action `build` has completed
4. Download `firmware` from completed action

## Generating svg image

### Step 0, move into keyboard folder

### Step 1, generate YAML:

```bash
keymap parse -z piantor_pro_bt.keymap > piantor_pro_bt_keymap.yaml
```

### Step 2, draw svg:

```bash
keymap -c ../../../keymap-drawer-config.yaml draw -k beekeeb/piantor_pro -l LAYOUT_split_3x6_3 piantor_pro_bt_keymap.yaml > piantor_pro_bt_keymap.svg
```

convert from qmk to zmk:
https://github.com/aaronsantiago/qmk-to-zmk/blob/main/index.html

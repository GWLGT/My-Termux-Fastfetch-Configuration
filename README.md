# What is This?

This is just my Configuration file for [Fastfetch](https://github.com/fastfetch-cli/fastfetch/).. that't it.

# Note

If you have Mesa Package installed, make sure to put `LD_LIBRARY_PATH="/vendor/<arch-lib>:/system/<arch-lib>"` **(change `<arch-lib>` to folder based on your CPU Bit, e.g, `lib/` for 32 Bit, `lib64/` for 64 Bit)**, so the command becomes:

```bash
LD_LIBRARY_PATH="/vendor/<arch-lib>:/system/<arch-lib>" fastfetch
```

If you don't, Fastfetch will fetch **Wrong** OpenGL/OpenCL and your GPU Information.

And, make sure to Put this Code in your Shell rc file:

```bash
if [[ -n "$DISPLAY" ]]; then
  export WM="Openbox" # Change to your Window Manager Name
  export DE="None" # Change to your Desktop Environment Name
  export DET="Slot Dark (Kvantum)" # Change to your DE/WM Theme
  export DEF="DejaVu Sans" # Change to your DE/WM Font Name
  export DEW="$HOME/.wallpaper/Cosmos-planets-Universe.jpg" # Change to your DE/WM Wallpaper Path
else
  export WM="None"
  export DE="None"
  export DET="None"
  export DEF="None"
  export DEW="None"
fi
```

so the Last Section of the Fastfetch Output show Correct Information.

Easy "clone and go" repository for a libopencm3 based project.

# Instructions
 1. git clone --recurse-submodules https://github.com/iXhong/libopencm3-template.git your-project
 2. cd your-project
 3. make -C libopencm3 # (Only needed once)
 4. make -C app

If you have an older git, or got ahead of yourself and skipped the ```--recurse-submodules```
you can fix things by running ```git submodule update --init``` (This is only needed once)

# Directories
* app contains your application
* shared contains something shared.

# Make & Flash
* once you have code in dir /app, 
* ```cd app``` change the workdir
* ```make bin``` make the bin file
* ```st-flash write your_bin.bin 0x8000000```

# As a template
You should replace this with your _own_ README if you are using this
as a template.

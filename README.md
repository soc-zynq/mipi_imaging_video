# mipi_imaging_video

## Description
A simple kernel module with a user-space application.

## Project Structure
```
mipi_imaging_video/
├── kernel_module/
│   ├── src/
│   │   └── mipi_imaging_video.c
│   ├── include/
│   │   └── mipi_imaging_video.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd mipi_imaging_video/kernel_module
make
```

### Application
```bash
cd mipi_imaging_video/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod mipi_imaging_video/kernel_module/mipi_imaging_video.ko
# Do something with the module
sudo rmmod mipi_imaging_video
```

### Application
```bash
cd mipi_imaging_video/application
./test_app
```

## License
GPL

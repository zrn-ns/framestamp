# FrameStamp

A script that adds borders to photos and displays EXIF information.

This script is inspired by [Sukashi App](https://play.google.com/store/apps/details?id=app.sukashi&hl=ja).

| Before | After |
| ------- | ------- |
| <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/3b9340cf-d6c2-4769-a83a-caf739690802" /></kbd> | <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/b757bbc0-dd0c-4eea-8850-762637470ea6" /></kbd> |
| <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/d69368b5-cef0-49d1-ae38-6e59260da877" /></kbd> | <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/06d043d5-ca92-40a0-8285-af943dfe555e" /></kbd> |
| <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/fe7c12e6-6e94-46e0-b088-380c02b6faa8" /></kbd> | <kbd><img width="500px" src="https://github.com/zrn-ns/framestamp/assets/5319256/44625352-466e-494d-91f7-c3103059b5d5" /></kbd> |

## Usage

Test environment: macOS 14.0 (23A344)

#### 1. Check out this repository and navigate to its directory

```sh
git clone https://github.com/zrn-ns/framestamp.git
cd framestamp
```

#### 2. Install GNU parallel

```sh
brew install parallel
```

#### 3. Add input images to the input directory

```sh
cp /path/to/image.jpeg ./input/
```

#### 4. Execute the script

```sh
./framestamp

# The generated files will be output to the output directory
ls -alF output
```

## Notice

- Images are force-resized.
- Images are processed in parallel.

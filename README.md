# panoramas-image-stitching

Forked from [panoramas-image-stitching](https://github.com/SSARCandy/panoramas-image-stitching)

## Requirement

- python3 (or higher)
- opencv 3.0 (or higher)

You will need to install some package using `pip3`:

- numpy
- matplotlib

Install using `pip3 install -r requirements.txt`     

## Usage



```bash
$ cd src
$ python main.py <input img dir>

# for example
$ python ./main.py ../input_image/Synthetic/
```

## Input format

The input directory should have:

- Some `.png` or `.jpg` images
- A `image_list.txt`, file should contain:
  - filename
  - focal_length

This is an example for `image_list.txt`:

```
# Filename   focal_length
img184.jpg 1320
img185.jpg 1320
img186.jpg 1320
img187.jpg 1320
img171.jpg 1320
img172.jpg 1320
img173.jpg 1320
img174.jpg 1320
img175.jpg 1320
img176.jpg 1320
img177.jpg 1320
img178.jpg 1320
img179.jpg 1320
img180.jpg 1320
img182.jpg 1320
img183.jpg 1320
```


## Output

The program will store the following images in the result directory:

- Every stitched images, with filename `0.jpg`, `1.jpg`, `2.jpg`, ...
- A aligned image `aligned.jpg`
- A cropped image `cropped.jpg`

## Parameters

The program have some constant parameters that can easily changed in `constant.py`.

## Environment

Code tested in Windows/Linux/MacOS

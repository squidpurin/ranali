+++
date = 2020-12-27T07:59:00Z
draft = true
tags = ["test"]
title = "My Second Post"

+++
# Test Heading

## Test Subheading

This is a test post to check for layout for the website.'

## Some Lorem Ipsum stuff

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et **dolore magna aliqua**. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit _esse cillum_ dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Images maybe

![](/uploads/ranaface.jpg)

## Codeblock test

    def jpeg_res(filename):
       """"This function prints the resolution of the jpeg image file passed into it"""
    
       # open image for reading in binary mode
       with open(filename,'rb') as img_file:
    
           # height of image (in 2 bytes) is at 164th position
           img_file.seek(163)
    
           # read the 2 bytes
           a = img_file.read(2)
    
           # calculate height
           height = (a[0] << 8) + a[1]
    
           # next 2 bytes is width
           a = img_file.read(2)
    
           # calculate width
           width = (a[0] << 8) + a[1]
    
       print("The resolution of the image is",width,"x",height)
    
    jpeg_res("img1.jpg")

This is code for something.
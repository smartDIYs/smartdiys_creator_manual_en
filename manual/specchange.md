We will explain the main specifications that have been changed from the current ***FABOOL Desktop***

## Change raster image import DPI
Until now, raster images were read as 90dpi when reading, but this was changed to 254dpi. This specification change affects only the size at which the object is placed at import (it is placed smaller), not the number of pixels retained. However, both FABOOL Desktop and SmartDIYs Creator will be resized to 1023 pixels and imported if the resolution in the x direction exceeds 1023 pixels.

## Change of raster image processing method
In the past, scaling was used to change the engraving density (DPI) at the time of processing due to scaling of the image and affect the processing results. However, regardless of scaling, specification to keep DPI at processing time has been changed. "DPI at processing time" indicates how much definition the read image data is irradiated with laser light. In other words, it is the definition when dithering the grayscale image. However, due to the limitations of the current firmware, the maximum number of dots in the x direction will be 1023, and if this is exceeded, it will be expressed scaled in the x direction. In addition, since the scan interval in the Y direction also changes with DPI, it is possible to shorten processing time by lowering DPI and processing.

```
※ The following images are engraved with the same image data and the same processing size.   
※ It can be set individually according to the characteristics of the material and processing time efficiency.   
※ Engrave cardboard with FABOOL Laser Mini 3.5W / Use image: 1023 × 778 pixels
```

<p align="center">
<img alt="SmartScreen" src="./images/specchange/rasterDPI.jpg" style="width:80%">
</p>

## Changed some interpretation of SVG reading.
Until now, lines were automatically added to Fill data created only with "painting", but this specification has been changed so that lines are not automatically added. This specification change is intended to prevent the concept from becoming complicated. Due to this specification change, the same SVG data may cause differences in import results compared to FABOOL Desktop.

## Changed the optimization at the time of FILL processing
The application of route optimization (shortest route) at the time of Fill object processing has been discontinued, and it has become a specification that it will be sequentially processed in the Y-axis direction like a raster. As a result, processing time may increase with some data, but risks such as axis slippage due to lack of hardware adjustment are reduced.

## Behavior change at copy & paste
In the past, when copying and pasting objects, parameter setting items are also duplicated, and it was difficult to change numerical numbers. With this change of specification, copied and pasted objects will share the same parameters. If you want to set another parameter as before, import the image file etc. again.

There are other minor differences in operation, but the basic idea is the same as the current FABOOL Desktop.

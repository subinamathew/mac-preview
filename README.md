# mac-preview scan without reducing quality
How to decrease .pdf size without losing quality in mac preview scanner? 

Source: https://apple.stackexchange.com/questions/297417/how-to-decrease-pdf-size-without-losing-quality

If you are struggling to get a scan for indian visa that says that the passport copy must be less than 300KB then this is the best way around.

This will help you reduce the scanned pdf with reduced quality.

This is done by adding a custom filter. 

In Mac, scanned images can be exported as PDF by using `Export as PDF` button or `Export` button.

The `Export` button has so many choices. One of them is reduced PDF. But this messes up the image size. Here is the way around it.

Enjoy

## Adding custom filter step by step
- Create new directory (if you don't have it) - /Library/Filters
  
  `mkdir /Library/Filters`
    
- Add there new filter file with unique filter - f.e. Reduce Size with good quality.qfilter

  `touch ReducedFilter.qfilter`
  `touch ReallySmall.qfilter`

The file should contain XML with new filter - you can base on the /System/Library/Filters/Reduce.qfilter file.

Change compression setting, image size and add unique display name for your filter.

See the filters attached.

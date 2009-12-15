## NSDate (RelativeDate)
A category to extend Cocoa's NSDate class with relative date function

### How to use
To use it in your Cocoa project, import the header and implementation files, and then add the header to your project’s _prefix.pch file so that it’s available across your project:

    #ifdef __OBJC__
        #import <Foundation/Foundation.h>
        #import <UIKit/UIKit.h>
        #import "NSDate+Helper.h"
    #endif

And in your source:

    NSDate *date = [NSDate date];
    NSString *relativeDate = [date relativeDate];

That's it. 

The output format is *relativeNumber+firstCharOfTheDateUnit*, such as "**now**", "**1s**" (one second ago), "**2d**" (two days ago), "**3w**" (three weeks ago), "**4m**" (four months ago), "**5y**" (five years ago), etc.
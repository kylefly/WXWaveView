# WXWaveView

[![](https://img.shields.io/badge/platform-iOS-orange.svg)](https://developer.apple.com/ios/)
[![](https://img.shields.io/badge/pod-1.0.1-brightgreen.svg)](https://github.com/CocoaPods/CocoaPods)
[![](https://img.shields.io/badge/carthage-compatible-red.svg)](https://github.com/Carthage/Carthage)
[![](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/WelkinXie/WXWaveView/blob/master/README.md)

### Add pretty and smooth waves to your views! 

#### The wave can be added to any type of view.

#### [中文说明](https://github.com/WelkinXie/WXWaveView/blob/master/README-CN.md)

e.g.

![](https://raw.githubusercontent.com/WelkinXie/WXWaveView/master/wave.gif)

## Integration
Cocoapods:

```
pod 'WXWaveView'
```

Or Carthage:

```
github "WelkinXie/WXWaveView"
```

## How to use
1. Initialize WXWaveView with method " **addToView:withFrame:** "
	
		self.waveView = [WXWaveView addToView:headerView withFrame:CGRectMake(0, CGRectGetHeight(headerView.frame) - 10, CGRectGetWidth(headerView.frame), 10)];
	
	Of course, you can just give CGRectZero to the method above and use __Auto Layout__ to define its frame.

2. Perform the method **wave** when you want it to animate.

		[self.waveView wave];

That's it!

## Customization
1. The time when the wave lasts. When it is set to zero, the wave will never stop. Default is 1.5.

	    self.waveView.waveTime = 0.f;  
	    
2. The color of the wave. Default is white.
	    
	    self.waveView.waveColor = [UIColor groupTableViewBackgroundColor];
	   	
3. The speed of the wave. Default is 9.

	    self.waveView.waveSpeed = 20.f;
	    
4. The angular speed of the wave. Default is 2.

		self.waveView.angularSpeed = 1.8f;
	    
5. You can also stop the wave manually with the method **stop** whenever you want.

		[self.waveView stop];
		
#### Recently I find it amusing to make it a loading view ：

![](https://raw.githubusercontent.com/WelkinXie/WXWaveView/master/wave2.gif)

What will it be depends on your creativity! Have fun :]
	    
## Reference
**WXWaveView** is inspired by [KYWaterWaveView](https://github.com/KittenYang/KYWaterWaveView). Thanks KittenYang and his contributions.

## License
**WXWaveView** is released under [**MIT License**](https://github.com/WelkinXie/WXWaveView/blob/master/LICENSE).
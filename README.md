# JHSlider
A slider which can tracking current value.

### Simple to use

#### example:

```
    CGRect bounds = [UIScreen mainScreen].bounds;
    CGFloat X = 100, Y = 200, W = bounds.size.width - 2*X, H = 40;
    CGRect frame = CGRectMake(X,Y,W,H);
    
    JHSlider *slider = [[JHSlider alloc] initWithFrame:frame];
    slider.value = 30;
    slider.minimumValue = 0;
    slider.maximumValue = 100;
    slider.backgroundColor = [UIColor brownColor];

    slider.trackingLabel.frame = CGRectMake(50, 0, 50, 20);
    slider.trackingLabel.backgroundColor = [UIColor grayColor];
    slider.trackingLabel.textAlignment = 1;
    slider.trackingLabelTextFormat = @"%.0f%%";
    slider.trackingLabelOffsetY = 15;
    
    slider.trackingBackgroundView.frame = CGRectMake(10, 10, 60, 30);
    slider.trackingBackgroundView.backgroundColor = [UIColor greenColor];
    slider.trackingBackgroundViewOffsetX = -5;
    
    slider.leftLabel.hidden = NO;
    slider.leftLabel.backgroundColor = [UIColor lightGrayColor];
    
    slider.leftView.hidden = NO;
    slider.leftView.backgroundColor = [UIColor purpleColor];
    
    slider.rightLabel.hidden = NO;
    slider.rightLabel.backgroundColor = [UIColor lightGrayColor];
    
    slider.rightView.hidden = NO;
    slider.rightView.backgroundColor = [UIColor purpleColor];
    
    [slider setThumbImage:[UIImage imageNamed:@"btn_adjust"] forState:0];
    
    [self.view addSubview:slider];
    
```
### a image may help you
![image](https://github.com/xjh093/JHSlider/blob/master/JHSlider.png)

### a gif image
![image](https://github.com/xjh093/JHSlider/blob/master/JHSlider.gif)

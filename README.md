# shch

  UIImage* image3 = [UIImage imageNamed:@"mail-48_24.png"];
  
 CGRect frameimg = CGRectMake(0, 0, image3.size.width, image3.size.height);
 
 
 UIButton *someButton = [[UIButton alloc] initWithFrame:frameimg];
 
 
[someButton setBackgroundImage:image3 forState:UIControlStateNormal];

[someButton addTarget:self action:@selector(sendmail)

     forControlEvents:UIControlEventTouchUpInside];
     
[someButton setShowsTouchWhenHighlighted:YES];

UIBarButtonItem *mailbutton =[[UIBarButtonItem alloc] initWithCustomView:someButton];

self.navigationItem.rightBarButtonItem=mailbutton;  

2. Add a ViewControllerBasedStatusBarAppearance Boolean key if it is not existing and assign value “NO”.

3. // Change the appearance of back button  ******

    UIImage *backButtonImage = [[UIImage imageNamed:@"button_back"] resizableImageWithCapInsets:UIEdgeInsetsMake(0, 13, 0, 6)];
    
    [[UIBarButtonItem appearance] setBackButtonBackgroundImage:backButtonImage forState:UIControlStateNormal barMetrics:UIBarMetricsDefault];
 
    // Change the appearance of other navigation button   ******
    
    UIImage *barButtonImage = [[UIImage imageNamed:@"button_normal"] resizableImageWithCapInsets:UIEdgeInsetsMake(0, 6, 0, 6)];
    
    [[UIBarButtonItem appearance] setBackgroundImage:barButtonImage forState:UIControlStateNormal barMetrics:UIBarMetricsDefault];
    
4.https://www.appcoda.com/customize-navigation-status-bar-ios-7/   ****

5.self.navigationItem.leftBarButtonItem=[self backButton];

  - (UIBarButtonItem *)backButton
  {
   UIImage *image = [UIImage imageNamed:@"image.png"];
   
   CGRect buttonFrame = CGRectMake(0, 0, image.size.width, image.size.height);

   UIButton *button = [[UIButton alloc] initWithFrame:buttonFrame];
   
   //[button addTarget:self action:@selector(backButtonPressed) forControlEvents:UIControlEventTouchUpInside];
   
   [button setImage:image forState:UIControlStateNormal];

   UIBarButtonItem *item= [[UIBarButtonItem alloc] initWithCustomView:button];

   return item;
 }
 
6.http://stackoverflow.com/questions/21252194/navigation-bar-button-item-image-color-is-different-when-design-through-xib-of-x   -  navigation 

7. http://stackoverflow.com/questions/22767098/how-to-change-inactive-icon-text-color-on-tab-bar - tabbar

8.https://teamtreehouse.com/library/implementing-designs-for-iphone/implementing-custom-login-and-sign-up-screens/adding-background-images-and-positioning-views  - check ui Appearence


/// -------------------///

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

  related SND
  
  1.  http://policyandsafety.help.soundcloud.com/customer/portal/articles/2155833-reporting-trademark-infringement   - check details
  
2. http://payments.help.soundcloud.com/?b_id=10245  - Payments & Bills

3. http://stackoverflow.com/questions/14848801/start-playing-soundcloud-audio-stream-in-ios-by-using-a-pre-buffer   - Start playing SoundCloud audio stream in iOS by using a pre-buffer   ------ imp  *******

4. http://stackoverflow.com/questions/18245805/not-playing-sounds-from-stream-url-ing-soundcloud-api   -  Not playing sounds from stream_url ing SoundCloud API

5. http://stackoverflow.com/questions/21177594/soundcloud-ios-api-playing-sound-from-link  - Soundcloud iOS API - playing sound from link

6. http://stackoverflow.com/questions/15537080/playing-a-soundcloud-file-in-ios-app -  Playing a SoundCloud file in IOS app

7 .http://stackoverflow.com/questions/23676831/stream-audio-with-avplayer  -  Stream  Audio with AVPlayer  ------------- Imp

8. http://bazookabyte.me/2014/05/01/quick-soundcloud-streams-with-avplayer/ - Quick SoundCloud Streams With AVPlayer ----- check

9. http://stackoverflow.com/questions/14086762/ios-soundcloud-stream-from-other-users    - soundCloud API ******

/// -------------------------//

  Showing Indicator
  
    1.  http://stackoverflow.com/questions/24114271/how-to-display-activity-indicator-in-song-loading-time-in-ios  -  How to display Activity Indicator in song loading time in iOS
    
2. http://stackoverflow.com/questions/22979376/how-to-display-loading-indicator-in-avaudioplayer-if-user-clicks-the-play-button  - how to display loading indicator in AVAudioPlayer if user clicks the play button

3. http://stackoverflow.com/questions/28579779/how-to-show-or-hide-activity-indicator-in-song-loading-time-in-ios/28580482#28580482  - How to show or hide activity indicator in song loading time in ios

4. http://stackoverflow.com/questions/16206893/adding-activity-indicator-while-avplayer-gets-ready-to-play-music  -   Adding activity indicator while AVplayer gets ready to play music  -------- imp ****

5.  http://webcache.googleusercontent.com/search?q=cache:http://qaoverflow.com/question/how-to-show-or-hide-activity-indicator-in-song-loading-time-in-ios/   -  check


6. http://stackoverflow.com/questions/30300435/what-is-the-proper-way-to-display-a-loading-indicator-while-getting-data-from-a  -  What is the proper way to display a loading indicator while getting data from a URL  - check

7. http://ebanshi.cc/questions/4816064/how-to-display-activity-indicator-in-song-loading-time-in-ios  -  How to display Activity Indicator in song loading time in iOS  - imp  ****

/// ------------------------//

  SND GTHB
  
    1. <https://github.com/soundcloud/CocoaSoundCloudAPI - soundcloud/CocoaSoundCloudAPI>
    
2. https://github.com/NextFaze/soundcloud-player-webview -   NextFaze/soundcloud-player-webview

3. https://github.com/soundcloud/soundcloud-custom-player  - soundcloud/soundcloud-custom-player




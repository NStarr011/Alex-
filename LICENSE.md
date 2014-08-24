 {
24	24	     // Sent when the application is about to move from active to inactive state. This can occur for certain types of temporary interruptions (such as an incoming phone call or SMS message) or when the user quits the application and it begins the transition to the background state.
25	25	     // Use this method to pause ongoing tasks, disable timers, and throttle down OpenGL ES frame rates. Games should use this method to pause the game.
26		-    
27		-    wipeAll();
28	26	 }
29	27	 
30	28	 - (void)applicationDidEnterBackground:(UIApplication *)application
31	29	 {
32	30	     // Use this method to release shared resources, save user data, invalidate timers, and store enough application state information to restore your application to its current state in case it is terminated later. 
33	31	     // If your application supports background execution, this method is called instead of applicationWillTerminate: when the user quits.
34		-    wipeAll();
35	32	 }
36	33	 
37	34	 - (void)applicationWillEnterForeground:(UIApplication *)application
...	...	@@ -51,7 +48,6 @@ - (void)applicationDidBecomeActive:(UIApplication *)application
51	48	 - (void)applicationWillTerminate:(UIApplication *)application
52	49	 {
53	50	     // Called when the application is about to terminate. Save data if appropriate. See also applicationDidEnterBackground:.
54		-    wipeAll();
55	51	 }
56	52	 
57	53	 @end

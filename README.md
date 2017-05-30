# DKNavigationDrawer
Navigation Drawer for iOS using Swift. 
Add DKNavDrawerDelegate, DrawerView and DrawerView to project.
Assign class DKNavDrawer to your navigation controller
Add a Right Bar Button to your RootViewController connect it to a action.
RootViewController should conform to DKNavDrawerDelegate
Initialize -  var rootNav: DKNavDrawer?
 

In viewDidLoad() of RootViewController add 2 lines  
 rootNav = (navigationController as? DKNavDrawer)
 rootNav?.dkNavDrawerDelegate = self


The button action me
@IBAction func btnToggle(_ sender: Any) {
          rootNav?.drawerToggle()
    }
    //Implement this as this is a delegate method
       func dkNavDrawerSelection(_ selectionIndex: Int) {
    }

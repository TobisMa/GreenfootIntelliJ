# GreenfootIntelliJ

**NOTE**: 
   - The used paths for configuration are only valid on windows
   - Requires greenfoot to be at `C:\Program Files\Greenfoot\**`
   - Requires [combined greenfoot sources](https://github.com/Rc-Cookie/greenfoot-sources-combined) to be at `C:\Program Files\greefoot-sources-combined-main`
   - The above paths can be changed in the GreenfootLibs library in the Project Structured

## How to use
1. Create a new repository using the button `Use this template` and create a new repository
2. Open IntelliJ locally and open the project using IntelliJ's VCS integration and your git repository URL
3. Add the GreenfootLibs to your projects module dependencies
   1. Open `File > Project Structure...`
   2. Go to `Libraries`
   3. Right click on `GreenfootLibs`
   4. Click on `Add to Modules...`
   5. Confirm by pressing on Apply/Ok in the right bottom corner
4. Make a test run by running the configuration `Run Scenario`

## Changing entry point
### Default entry point
- constructor in `MainWorld.java` which extends `greenfoot.World`

### Changing entry point
1. Create your own java class or rename the class in the `src` directory if not already done
2. Make sure your class is extending `greenfoot.World`
3. Go to the file `src/standalone.properties` and search for `main.class`
4. Change the class name in the line and (re)start your greenfoot project to your class name

### Can I still you use greenfoot?
Yes, you can still use greenfoot. Just go to into your file explorer to the projects directory and open the project on `src/project.greenfoot`.  
Optionally, you can start greenfoot and open a project using the `src` folder. In greenfoot all features are still available, and you can switch between IntelliJ and greenfoot as you would like to.

### Tips when working in a team
 - use the setImage function within Actors for the images to be on the safe side when working in a team (ensures no failures when merging the project.greenfoot file)
 - use the setBackground function in world
 - use above functions once in the constructor to have an image set intially (otherwise greenfoot's foot will be used as placeholder)
 - adding objects to a world can be a bit bothersome, so you could use greenfoot for that anyway. But you can do it in the world, as well
 - greenfoot has templates like Counter, etc. but you need to use the greenfoot application to import those or just make them yourself

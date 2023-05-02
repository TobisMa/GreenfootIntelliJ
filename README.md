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

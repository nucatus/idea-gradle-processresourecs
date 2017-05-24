# idea-gradle-processresourecs

## The issue

When running this project from IntelliJ, the gradle `processResources` task is not correctly handled. 
This task has a dependency that is not executed when the IntelliJ Run/Debug procedure prehandles this gradle `processResources` task.

### Expected behavior

The content of the `src/main/scripts` folder should be copied to `build/scripts` folder.

### Observed behavior

The content of the `src/main/scripts` folder is NOT copied to `build/scripts` folder.

If I run this task manually with `gradle processResources`, the expected behavior is observed.

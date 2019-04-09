#Which one to use Shared (.so) or static (.a) libraries?


When you create a shared .so library, it basically copies all the .a files that you added in the target_link_libraries(). However
when you create a static .a library, it doesn't copy the .a files that you added in the target_link_libraries(), in fact, target_link_libraries() does nothing. So in the final executable you
have to add as target_link_libraries().

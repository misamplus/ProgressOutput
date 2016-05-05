Progress Output
==========

The Asynchronous Progress Output For JAVA

Contents
==============================

1. <a href="#1-detail--contact">Detail & Contact</a>
2. <a href="#2-how-to-use">How To Use</a>
3. <a href="#3-license">License</a>

1. Detail & Contact
==============================

* Name: Progress Output
* Version: 1.0
* Author: Misam Saki, http://misam.ir/
* Document: https://github.com/misamplus/ProgressOutput

2. How To Use
==============================

1. Add ProgressOutput.java to your code.
2. Extend your object class from ProgressObject.
   <pre>
    ... class [Your Class Name] extends ProgressObject {
   </pre>
3. Create a new ProgressOutput object and pass your object class to it!
   <pre>
    ProgressOutput progressOutput = new ProgressOutput(this);
   </pre>
4. Start ProgressOutput.
   <pre>
    progressOutput.start();
   </pre>
5. Now you can change `percent` variable in your class to update it in console.
   <pre>
    this.percent = 99;
   </pre>

3. License
==============================

Copyright © 2000 Misam Saki <hi@misam.ir>

This work is free. You can redistribute it and/or modify it under the

terms of the Do What The Fuck You Want To Public License, Version 2,

as published by Sam Hocevar. See the COPYING file for more details.

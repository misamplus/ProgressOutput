/**
 * The Asynchronous Progress Output For JAVA
 *
 * @version 1.0
 * @author Misam Saki, http://misam.ir/
 * @document https://github.com/misamplus/ProgressOutput
 *
 * Copyright © 2000 Misam Saki <hi@misam.ir>
 * This work is free. You can redistribute it and/or modify it under the
 * terms of the Do What The Fuck You Want To Public License, Version 2,
 * as published by Sam Hocevar. See the COPYING file for more details.
 */

public class ProgressOutput implements Runnable {
    private Thread thread;
    private ProgressObject obj;
    private int percent = -1;
    
    ProgressOutput (ProgressObject obj) {
    }
    
    public void run() {
        try {
            while (percent < 100) {
                if (percent != obj.percent) {
                    System.out.print((Integer.toString(percent) + "%").replaceAll(".", "\b"));
                    System.out.flush();
                    Thread.sleep(500);
                    percent = obj.percent;
                    String percentStr = Integer.toString(obj.percent) + "%";
                    System.out.print(percentStr);
                    System.out.flush();
                }
                Thread.sleep(1000);
            }
        } catch (InterruptedException ex) {
            System.err.println(ex.getMessage());
        }
        System.out.println();
    }
   
    public void start () {
        if (thread == null) {
            thread = new Thread(this);
            thread.start();
        }
    }
}

class ProgressObject {
    static int percent = 0;
}

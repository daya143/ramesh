# ramesh   


                    Moving ball code


import java.awt.*;
import javax.swing.*;
import java.lang.Thread;
import java.lang.*;
 
public class MovingBall extends JApplet
{
Thread t;
int i;
int x=34,y=14;
 
public void init()
{
t=new Thread();
}
public void paint(Graphics g)
{
for(i=1;i<=5;i++)
{
g.fillOval(x,y,40,40);
//g.setColor(Color.red);
x=x+30;
y=y+30;
repaint();
 
try
{
t.sleep(1000);
}
catch(Exception e)
{}
}
}
 
 
}

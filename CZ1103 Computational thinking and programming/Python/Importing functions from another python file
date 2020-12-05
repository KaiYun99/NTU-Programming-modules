# Coding Exercise 6a
# Write a function get_color(color) that takes a string parameter, “color” as the input
# and return the integer value of the color entered by the user, based on the code snippet
# given on page 2.
# The function checks for valid value entered by the user, in the range from 0 to 255.
# The function returns the valid value entered by the user
# If the user does not enter a valid value after 3 tries, the function will return a default
# value of 0  

from sense_hat import SenseHat
sense = SenseHat()
sense.set_rotation(0)

def get_color(color):
  
  keep_looping = True
  no_of_tries = 1
  
  while keep_looping:
    if no_of_tries <= 3:
      
      color_str=input("Enter the value of the " + color + "color for message (0 to 255):")
      if color_str.isdigit():
        if int(color_str) >= 0 and int(color_str) <= 255:
          return int(color_str)
        else:
          no_of_tries += 1
      else:
        no_of_tries += 1

    else:
      color = 0
      return color
    

r_int = get_color("red")
g_int = get_color("green")
b_int = get_color("blue")
msg_color = (r_int, g_int, b_int)
sense.show_message("I got it!", text_colour=msg_color)

#Coding Exercise 6b
# The function can be made into a sharable module such that it can be imported into a program


from textcolor.py import get_color        # Create a new python file in same directory (i.e both python files in same subfolder) textcolor.py is the file u importing from
import textcolor                          # May need to trial and error , if doesn't work , try removing " .py "  
                                          # Not sure if they will work , both works? or both don't work ? Any work ?
textcolor.get_color()
#then can use the function alr

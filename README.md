# HW5-567

While pylinting my triangle program, it was interesting how strictly pylint followed the snake_case naming style. For the function inputs, I simply had a, b, and c as the variables for the sides. To conform to the naming style, I change the variable names to side_a, side_b, and side_c respectfully. Pylint also brought to my attention how common I had trailing white space, with over 10 instances of the error. The most insightful thing I discovered while pylinting the triangle program is that instead of verifying the input using ``isInstance(side_a, int) or isInstance(side_a, float)``, I could optimize this by using ``isInstance(side_a, (int, float))``. I thought this was neat, and it made my program much more readable.

When checking the coverage of my unit tests, I was surprised to find that I had already achieved 100% coverage, according to the coverage python module. Reading through the coverage tutorial web page, I was able to generate a web page to better display the results. I put the source code of the web page in this repository as well.

This is the pylint output of the original program Triangle.py
![image](https://user-images.githubusercontent.com/56331076/136674414-426061e4-e354-4a06-80e6-ef90be93f5d4.png)

This is the pylint output of the improved program triangle_improved.py
![image](https://user-images.githubusercontent.com/56331076/136674482-d51d54e8-c4fa-4008-98b8-79d59b42eaf2.png)

This is the HTML output of the coverage test
![image](https://user-images.githubusercontent.com/56331076/136674580-50a4c7b9-f9e3-4f2a-97c8-04cdd824fb23.png)

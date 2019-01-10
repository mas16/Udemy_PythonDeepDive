"""
Section 2, Lecture 13

Classes: Review

Decorators: Getters and Setters

"""


class Rectangle:

    # Initialize attributes of class for object self
    def __init__(self, width: float, height: float):
        self._width = width
        self._height = height

    @property
    def width(self):
        return self._width

    @width.setter
    def width(self, width):
        if width <= 0:
            raise ValueError("Width must be positive number")
        else:
            self._width = width

    @property
    def height(self):
        return self._height

    @height.setter
    def height(self, height: float):
        if height <= 0:
            raise ValueError("Height must be positive number")
        else:
            self._height = height

    # self.width, self.height will call @property setters
    def area(self):
        return self.width * self.height

    def perimeter(self):
        return 2 * (self.width + self.height)


test_r1 = Rectangle(20, 20)

test_r1.height = -100

print(test_r1.perimeter())

<!-----


----->



```
// Managing the GUI application
#include <QApplication>
// Creating clickable buttons 
#include <QPushButton> 

int main(int argc, char **argv)
{
// Create a QApplication object to manage the GUI application
 QApplication app (argc, argv); 

// Create a QPushButton object
 QPushButton button; 

// Create a QFont object with the font family set to "Courier"
 QFont font ("Courier"); 

// Set an icon for the button
 button.setIcon(QIcon::fromTheme("face-smile")); 

// Set text for the button
 button.setText("He/She is a Programmer\nint main(int argc, char** argv){}"); 

// Set a tooltip for the button
 button.setToolTip("click Me!"); 

// Set the font of the button's text
 button.setFont(font); 

// Set the size of the button's icon
 button.setIconSize(QSize(50, 50));

// Display the button on the screen
button.show(); 

// Start the event loop of the QApplication 
// and return the exit code of the application when it's closed
 return app.exec(); 
}

# FluidUI
<h3>A UI, state management component framework. <br/><br/>Free to use forever<h3>

![FluidLogo](https://github.com/petxmr/fluidui/assets/111649405/f04f90cb-f3bf-42d0-a273-1c7a1f264c6e)

# Components

* **Switches** `[2 different variants]`
* **Buttons**  `[2 different variants]`
* **Sliders** `[3 different variants]`
* **Chips**    `[15 different variants]`
* **Code**     `[3 different variants]`
* **Labels**
* **Dropdowns** `[6 different variants]`
* **Accordians**
* **Cards** `[2 different types: products, actions]`
* **Spinners** `[4 different variants]`
* **Radios** `[2 different types: single, group]`
* **Tabs**

![Screenshot 2023-08-03 171115](https://github.com/petxmr/fluidui/assets/111649405/cfa77fb4-f02d-473e-b1f6-1be71d7dd6b4)

# Usage

<h3>FluidUI offers a JS like syntax and structure, you can easily import components / services like this</h3>

```lua
import({ "Button", "ButtonGroup" }).from("@fluidui/components")
```

<h3>This will automatically place 'Button' and 'ButtonGroup' in the global environment.</h3>

<h3>Using components can be accomplished like this:</h3>

```lua
import({ "Button", "ButtonGroup" }).from("@fluidui/components");

Button({
    isDisabled = false,
    variant = "Default",
    text = "Button 1",
    events = {
        ["Activated"] = function() 
            print("Hello, world!")
        end
    }
});

ButtonGroup("horizontal", {
    Button({
      isDisabled = false,
      variant = "Primary",
      text = "Button 2",
      events = {
          ["Activated"] = function() 
              print("Hello, world!")
          end
      }
    });
    Button({
      isDisabled = false,
      variant = "Primary",
      text = "Button 3",
      events = {
          ["Activated"] = function() 
              print("Hello, world!")
          end
      }
    });
});
```

### Code Challenge: Create an XCUITest for a Simple Counter App

#### Objective:
Write an XCUITest to validate the functionality of a simple counter application. The test should cover incrementing and decrementing the counter value.

#### Requirements:
1. **Environment Setup:**
   - Ensure you have Xcode installed.
   - Create a new Xcode project CounterApp following the steps from the Counter App Source Code section.
   - Add the XCUITest framework to your project.

2. **App Functionality to Test:**
   - **Increment Counter:** There should be a button to increment the counter value.
   - **Decrement Counter:** There should be a button to decrement the counter value.
   - **Counter Display:** The current counter value should be displayed on the screen.

3. **Test Scenarios:**
   - **Increment the Counter:**
     - Tap the "Increment" button.
     - Verify the counter value increases by 1.
   - **Decrement the Counter:**
     - Tap the "Decrement" button.
     - Verify the counter value decreases by 1.

#### Instructions:
1. **Setup the XCUITest Target:**
   - Create a new XCUITest target in your Xcode project.
   
2. **Write the XCUITest:**
   - Open the `CounterAppUITests.swift` file (or create a new one if necessary).
   - Write the test cases to cover the scenarios described above.

3. **Run and Validate:**
   - Run your XCUITest to ensure it works as expected.
   - Validate that all tests pass successfully.

### Submission

1. **Push the project to a public GitHub repository.**
2. **Submit the repository URL.**

Example:
```markdown
Repository URL: [https://github.com/yourusername/CounterApp](https://github.com/yourusername/CounterApp)
```   

### Counter App Source Code

#### 1. Create a New Xcode Project
1. Open Xcode and create a new project.
2. Choose the template "App" under "iOS".
3. Name the project "CounterApp".
4. Ensure "Swift" is selected as the language, and "Storyboard" is chosen for the interface.

#### 2. Main.storyboard
Design your interface in the storyboard:

1. Drag and drop a `UILabel` to display the counter value. Set its `text` property to `0` and give it an accessibility identifier of `counterLabel`.
2. Drag and drop two `UIButton` elements for incrementing and decrementing the counter. Set their titles to `Increment` and `Decrement` respectively, and give them accessibility identifiers `incrementButton` and `decrementButton`.

#### 3. ViewController.swift
Replace the content of `ViewController.swift` with the following code:

```swift
import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var counterLabel: UILabel!
    
    private var counter: Int = 0
    
    override func viewDidLoad() {
        super.viewDidLoad()
        updateCounterLabel()
    }
    
    @IBAction func incrementButtonTapped(_ sender: UIButton) {
        counter += 1
        updateCounterLabel()
    }
    
    @IBAction func decrementButtonTapped(_ sender: UIButton) {
        counter -= 1
        updateCounterLabel()
    }
    
    private func updateCounterLabel() {
        counterLabel.text = "\(counter)"
    }
}
```

#### 4. Connecting UI Elements to Code
1. Open `Main.storyboard`.
2. Select the `ViewController` scene and open the Assistant Editor (two interlocking rings icon) to show `ViewController.swift` side by side.
3. Control-drag from the `UILabel` to the code to create an IBOutlet named `counterLabel`.
4. Control-drag from the `Increment` button to the code to create an IBAction named `incrementButtonTapped`.
5. Control-drag from the `Decrement` button to the code to create an IBAction named `decrementButtonTapped`.

#### 5. Adding Accessibility Identifiers
1. Select the `UILabel` and in the Identity Inspector, set the "Identifier" under "Accessibility" to `counterLabel`.
2. Select the `Increment` button and set the "Identifier" under "Accessibility" to `incrementButton`.
3. Select the `Decrement` button and set the "Identifier" under "Accessibility" to `decrementButton`.

### Running the App
1. Run the app on a simulator or a real device.
2. Ensure the counter increments and decrements correctly when the respective buttons are tapped.

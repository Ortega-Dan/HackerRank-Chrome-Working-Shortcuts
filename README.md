# HackerRank-Chrome-Working-Shortcuts

```javascript
// just paste all this script in chrome console (read it and understand it first) and hit enter then close the console
// then use it in hackerrank according to the comments in the following code
window.onkeydown = function (event) {

    // hit alt to run code
    if (event.keyCode === 18) {
        document.getElementsByClassName("hr-monaco-compile")[0].click();
    }

    // hit altGr to submit code and if confirmation was received of successful submission, hit it again to jump to next-challenge-in-order
    if (event.keyCode === 225) {

        let el = document.getElementsByClassName("challenge-link")[0]

        if (el != undefined) {
            el.click()
        } else {
            document.getElementsByClassName("hr-monaco-submit")[0].click();
        }
    }
}
```

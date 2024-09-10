# Working Example for Element Plus Issue #394

This is part of a bug report for [Element Plus](https://github.com/element-plus/element-plus). The issue is that the first item in the select box is not selected by default when the dropdown is opened using the arrow down key. This works in version 2.3.12 but not in version 2.8.2.  

To see the implementation of the select box, check the `src/App.vue` file.
In there the first element is selected using el-select's `navigateOptions('next')` function.

To see the working example, check the following repository: [Element Plus Issue Working Example #18239](https://github.com/element-plus/element-plus/issues/18239).

Bug report: [Element Plus Issue #18239](https://github.com/element-plus/element-plus/issues/18239)

### To reproduce the issue, follow the steps below:
1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm run dev` to start the development server.
4. Open your browser and navigate to the URL shown in the terminal.
5. Use the tab key to navigate to the select box.
6. Press the arrow down key to open the dropdown.
7. Now you see that the first item is selected by default. (this does not work for element-plus version 2.8.2)
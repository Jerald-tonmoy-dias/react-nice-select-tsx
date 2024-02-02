# React NiceSelect

React NiceSelect is a customizable, lightweight, and easy-to-use dropdown select component for React and Next.js. It is inspired by the jQuery Nice Selector but built specifically for React applications. This component removes any dependencies on jQuery and offers a simple and clean alternative for creating select dropdowns in your React projects.

# Installation

To use React NiceSelect in your project, you can install it via npm :

     npm install react-nice-select

**Make sure to also import the required stylesheet `nice-select.css` into your project.**

    @import  'react-nice-select/nice-select.css';
    @import  NiceSelect from "react-nice-select/NiceSelect";

# Usage

    import React from 'react';
    import NiceSelect from "react-nice-select/NiceSelect";
    import "react-nice-select/nice-select.css";

    const YourComponent: React.FC = () => {
      const options: Option[] = [
        { value: 'chocolate', label: 'Chocolate' },
        { value: 'strawberry', label: 'Strawberry' },
        { value: 'vanilla', label: 'Vanilla' },
      ];

      const handleChange = (value: string) => {
        // Handle the selected value
        console.log(value);
      };

      return (
        <NiceSelect
          options={options}
          onChange={handleChange}
          // other optional props
        />
      );
    };

    export default YourComponent;

# Props

- `options`: An array of objects with `value` and `label` properties representing the dropdown options.
- `defaultValue`: The default selected option for the dropdown.
- `onChange`: A callback function triggered when an option is selected.
- `wrapperClass`: Additional CSS classes for the select wrapper.

Feel free to customize the component further based on your project's needs.

# Inspired by

This package is inspired by the jQuery Nice Selector.

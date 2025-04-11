# Social Media Dashboard

## Description
 This project is a comprehensive social media dashboard composed of several key components that demonstrate fundamental concepts in React development. Each component has been carefully designed to handle specific data structures, styled using > modern CSS techniques, and tested to ensure they meet the project requirements. The dashboard includes a user profile display, a statistics section, a friend list, and a transaction history table, all driven by JSON data files.

## Components Overview

## 1. Profile Component 

The `Profile` component displays user information for a social media account. The component takes in several props to render details such as the username, social media tag, location, avatar, and activity statistics. These data are stored in the `user.json` file.

**Key Features:**
- Displays the user's avatar, name, and location.
- Shows user activity statistics like followers, views, and likes.
- Utilizes a structured layout with CSS for a clean and responsive design.

**Example Usage:**
```js
import user from 'path/to/user.json';

<Profile
  username={user.username}
  tag={user.tag}
  location={user.location}
  avatar={user.avatar}
  stats={user.stats}
/>
```

## 2. Statistics Component 

The `Statistics` component is designed to display a variety of statistics based on the provided data. The data is passed as props, allowing the component to dynamically render the statistics. The title prop is optional, and the stats prop contains an array of statistical data stored in `data.json`.

**Key Features:**
- Renders a title for the statistics section if provided.
- Displays each statistic with a label and percentage.
- Includes the option to dynamically generate background colors for each statistic.

**Example Usage:**
```js
import data from 'path/to/data.json';

<Statistics title="Upload stats" stats={data} />
<Statistics stats={data} />
```

## 3. FriendList Component 

The `FriendList` component shows a list of the user's friends, with each friend's online status clearly indicated. This component accepts a `friends` prop, which is an array of objects representing each friend, stored in `friends.json`.

**Key Features:**
- Displays each friend’s avatar, name, and online status.
- Changes the background color of the status indicator based on whether the friend is online or offline.
- Renders a flexible list that can accommodate any number of friends.

**Example Usage:**
```js
import friends from 'path/to/friends.json';
<FriendList friends={friends} />
```

## 4. TransactionHistory Component 


The `TransactionHistory` component displays a table of financial transactions, ideal for tracking activities in an internet banking application. The transactions are passed in as the `items` prop, sourced from the `transactions.json` file.

**Key Features:**
- Renders a table format with headers for transaction type, amount, and currency.
- Supports a variety of transaction types, amounts, and currencies.
- Provides a clean and accessible layout.

**Example Usage:**
```js
import transactions from 'path/to/transactions.json';

<TransactionHistory items={transactions} />
```

## Overview 

Through the development of these components, I gained valuable insights into React's component-based architecture, prop handling, and state management. I improved my understanding of how to efficiently structure and pass data between components using JSON files. Additionally, I enhanced my skills in CSS styling, particularly in creating responsive and visually appealing user interfaces.

Working on this project also taught me the importance of modular design and the reusability of components. By separating concerns and organizing the codebase into distinct, manageable parts, I was able to maintain clarity and reduce complexity as the project scaled.

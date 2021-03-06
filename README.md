# Inspiration
This project was inspired by my love for combining the visual with the technical. As a front-end developer, my job often relies on visual resources that need to be compared and quickly accessed. The concept of generating a "moodboard" is often the first step in my process. By isolating images within a board and displaying them in a configurable way, designers, developers, and marketers can use Monday.com in an entirely new context.

## What it does
Masonry view shows tiles representing every item on a board. Using the board settings, users can configure the view to show images from a "file" or "link" column. The users can also opt to hide items that do not contain images, or hide item names altogether to see only visuals.

## How I built it

I started this app using Monday's `quickstart-react` scaffolding, using my own React and front end experience to give it a unique twist.

## Challenges & Accomplishments

This was my first time using the Monday.com JavaScript SDK, so it took a bit of reading to get my footing and integrate information from the board in a meaningful way. Fortunately, I found the documentation very intuitive and was able to utilize the Monday Community forum to answer all my questions.

At the beginning of this challenge, I ran into issues with the `monday.execute()` command used to open item cards. After raising the issue in the Monday Community forum, the problem was tracked and a fix was implemented. I am proud that this collaboration lead to a long-term solution that could help future developers.

## What's next for Masonry View

I would love to expand this project to give users more granular control over what information is displayed on each card in the view. I could also see this view connecting with other inspiration sources, such as Pinterest or Behance.

# Developer Instructions

In the project directory, you should run:

### `npm install`

And then to run an application with automatic virtual ngrok tunnel, run:

### `npm start`

Visit http://localhost:4040/status and under "command_line section" find the URL. This is the public URL of your app, so you can use it to test it.
F.e.: https://021eb6330099.ngrok.io

## Configure Monday App

1. Open monday.com, login to your account and go to a "Developers" section.
2. Create a new "QuickStart View Example App"
3. Open "OAuth & Permissions" section and add "boards:read" scope
4. Open "Features" section and create a new "Boards View" feature
5. Open "View setup" tab and fulfill in "Custom URL" field your ngrok public URL, which you got previously (f.e. https://021eb6330099.ngrok.io)
6. Click "Boards" button and choose one of the boards with some data in it.
7. Click "Preview button"
8. Enjoy the Quickstart View Example app!

## Release your app

1. Run script

### `npm run build`

2. Zip your "./build" folder
3. Open "Build" tab in your Feature
4. Click "New Build" button
5. Click "Upload" radio button and upload zip file with your build
6. Go to any board and add your just released view
7. Enjoy!

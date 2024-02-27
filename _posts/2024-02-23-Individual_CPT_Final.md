---
toc: true
comments: true
layout: post
title: Advik Garg - Tri 2 Final Individial Review
description: Going over my individual feature(s), the overall project, and College Board requirements.
type: tangibles
courses: { compsci: {week: 1} }
---

# Project Overview
Our group wanted to make a video sharing site, similar to YouTube. Obviously this is a huge task, so we set our goals to the main concept of video sharing and viewing experience. Our site has user functionality with JWT, and roles to allow administrators to manage other users. We support video uploading/viewing with thumbnails and view counts.

# My Feature
I contributed to many parts of the project, but the individual feature I wanted to highlight was the main upload feature for each video, using user-submitted information to add videos to the database, and view them in the frontend.

[CB Requirements](https://apcentral.collegeboard.org/media/pdf/ap-csp-student-task-directions.pdf)

# Component A: Program

| CB Requirements | Me |
|-----------------|----|
| Instructions for input from one of the following: the user, a device, an online datas stream, a file. | Takes in the following information for the video: title, description, genre, video file, and thumbnail(image file). ![Code](https://i.ibb.co/z7jRXKd/image.png) |
| Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the users purpose. | We use an SQLite table to store everything besides the actual video file, which is statically served on the flask app in the /videos directory. All of this is connected through the database, making everything very streamlined and easily accessible. ![SQLite DB](https://i.ibb.co/wKbn37j/image.png) ![DB Init](https://i.ibb.co/qFpCtkH/image.png) |
| At least one procedure that contributed to the program’s intened purpose where you have defined: the name, return type, one or more parameters. | Code that creates a video in the database given metadata and a video file. ![Code](https://i.ibb.co/wwN90Jm/image.png) |
| An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure. | Our database initialization uses for loops and if statements to loop through a list of video objects to add to the database: ![Code](https://i.ibb.co/ypVMcyF/image.png) |
| Calls to your student-developed procedure. | Calls the create method in the POST request code in the Flask API endpoint. ![Code](https://i.ibb.co/F0bVnXH/image.png) |
| Instructions for output (tactile, audible, visual, or textual) based on input and program functionality | Success returns JSON of video: ![Code](https://i.ibb.co/yWNkfJw/image.png) |

# Component B: Video

[Link to Video](https://drive.google.com/file/d/1zlfNynV7jhEseaNGTBBQtMx_gxLN4kmW/view?usp=sharing)

| CB Requirements | Me |
|-----------------|----|
| Input to program | Uploading thumbnail and video file along with title, description, and genre. |
| At least one aspect of the functionality of your program | Viewing the video in the video player |
| Output produced by program | Home page updated with video |
| My video does not have | Voice narration |
| My video is | In .mp4 format, 1 minute in length, less than 30MB in file size |
# CreateSafe Technical Evaluation

## Project Summary

We often find ourselves on the receiving end of large (1GB+) video assets from artists that need to be rendered in our web applications. These files are in formats that are not capable of being played consistently across devices (mov, webm, etc.). Rather than asking the artist to compress, trim, and reformat the video files themselves we would like to do this automatically.

The tool you will be building is a basic web application for uploading video files that accepts any valid video file format, converts it to a MP4 file (with +faststart enabled), removes audio, and removes length from the end as needed to fit below 4.5mb.

## Solution Requirements

We recommend starting with [this template](https://github.com/theodorusclarence/ts-nextjs-tailwind-starter) for this project, and using vercel for hosting.

- Code must use typescript and react
- Output video file must be below 4.5mb
- Output video file must have no audio track
- Output video file must be a MP4 with +faststart enabled
- If trimming is required to fit the video below 4.5mb, it must trim from the end of the file
- Interface must allow users to upload an input video file from their local file system
  - Solution is expected to work with files of an arbitrary size
- Interface must show a preview of the output video file
- Interface must allow user to download the new output file
- Solution does not need to use an API - if you feel that you can accomplish this in some way solely as a front-end application, you may do so
- Feel free to use external services, keeping in mind cost of this application at scale

## Review Notes

Your solution to this problem will be rated on functionality, code structure and cleanliness, and overall usability (UX/UI) for end users. Please leave comments in your code describing any thoughts or notes that are relevant for our reviewer.
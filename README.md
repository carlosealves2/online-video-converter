
# Video Processing and Conversion System with Queue Communication

## Overview
This project aims to build a distributed system for processing and converting video files using queue-based communication. It integrates Docker, RabbitMQ, MongoDB, and Nginx for load balancing, providing a robust and scalable solution for video file handling.

## Features
- **Video Upload and Email Submission**: Users can upload video files along with an email address. The system stores these files either locally or in cloud storage.
- **Video Processing**: Videos are converted to specified formats using `ffmpeg`. The processing task is handled by a worker that reads messages from a processing queue.
- **Notification System**: Once the video processing is complete, the system updates the video status in the database and sends a notification email to the user.
- **Video Download**: Users can download the processed video by accessing a specific endpoint with the video's ID.
- **Real-time Media Listing (Optional)**: An endpoint to list all the media being processed, their status, and pre/post-processing information, with real-time updates via SSE or WebSocket.

## Architecture
- **Docker**: Containerization of the application components.
- **RabbitMQ**: Message queue for managing video processing tasks.
- **MongoDB**: Database for storing video metadata and processing status.
- **Nginx**: Load balancer for distributing incoming requests.

## Getting Started
Detailed instructions on setting up and running the project will be provided here, including steps to configure Docker, RabbitMQ, MongoDB, and Nginx.

## Prerequisites
List of prerequisites such as Docker, MongoDB, etc., will be detailed here.

## Installation
Step-by-step guide to install and configure the necessary tools and technologies.

## Usage
Instructions on how to use the system, including how to upload videos, monitor processing status, and download processed videos.

## Contributing
Guidelines for contributing to the project.

## License
Information about the project's license.

---

# Live Streaming Video Chat App (Without Voice) Using Socket Programming and OpenCV in Python

### 1. **Introduction**
This document outlines the process of creating a live streaming video chat application without voice, utilizing Python's OpenCV for video processing and socket programming for network communication. The application consists of a server and client program, both of which facilitate the transmission of video data over a network.

### 2. **Prerequisites**
- **Operating Systems:** 
  - Server: Red Hat Linux 8 (running on a virtual machine)
  - Client: Windows 10
- **Programming Language:** Python
- **Required Libraries:** 
  - `socket`: Provides two-way communication between the client and server.
  - `cv2`: Part of OpenCV, used for video capture and image processing.
  - `pickle`: Used for serializing and deserializing Python objects.
  - `struct`: Facilitates conversion between Python data types and C-compatible binary data.

### 3. **Server Program Overview**
The server is responsible for capturing video frames, processing them, and sending them to the client.

#### 3.1 **Library Installation**
Before running the server program, ensure that the required libraries (`socket`, `cv2`, `pickle`, `struct`) are installed in your Python environment.

#### 3.2 **Socket Creation**
For details on creating and binding the server socket, refer to the [server.py](Server.ipynb) file.

#### 3.3 **Handling Client Connections**
For details on accepting client connections and transmitting video frames, refer to the [server.py](Server.ipynb) file.

### 4. **Client Program Overview**
The client receives the video stream from the server, deserializes the data, and displays the video in real-time.

#### 4.1 **Socket Creation**
For details on creating and connecting the client socket, refer to the [client.py](Client.ipynb) file.

#### 4.2 **Receiving and Displaying Video**
For details on receiving and displaying video frames, refer to the [client.py](Client.ipynb) file.

### 5. **Key Points**
- **Socket Programming:** Sockets enable real-time communication between the client and server. The server listens on a specific IP and port, and the client connects to this endpoint.
- **OpenCV Integration:** OpenCV is used for video capture and processing. The server captures video frames, which are then transmitted to the client.
- **Data Serialization:** `pickle` is used to serialize the video frames (as NumPy arrays), and `struct` is used to pack and unpack the data, ensuring compatibility between Python and C.

### 6. **Conclusion**
This document provides an overview of the live streaming video chat application without voice, focusing on socket programming and OpenCV integration. The project demonstrates the basics of network communication and real-time video processing using Python.

I've created a YouTube video. Check it out!: https://youtu.be/NW3rgyFf9_8

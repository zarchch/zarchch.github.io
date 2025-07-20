---
layout: post
title: PicDisposal
author: Zhicheng Zhang
date: 2020-06-20 14:23:54 +0800
tags: [Project]
excerpt_separator: <!--excerpt-->
comments: true
sticky: false
---
This is an android application created for processing image. In this application, you can achieve various image processing such as **Convex**, **Concave**, **Nostalgia** and **Cartoon** within a short time period.<!--excerpt--> If you want to use the Android application, you should download and set up [./PicDisposal_py](https://github.com/ZZwarn1998/PicDisposal/tree/master/PicDisposal) and [./ImageDisposal](https://github.com/ZZwarn1998/PicDisposal/tree/master/ImageDisposal) additionally.  For more information, please visit [the repository](https://github.com/ZZwarn1998/PicDisposal).

## Usage
### Designate IP and Port

After you open the application, you should designate **IP address** and **Port**. Only if you type correct  **IP address** and **Port** can you go to the next section. **IP address** is the **IP** of your server running the java web program, [ImageDisposal](./ImageDisposal), and **Port** is corresponding **port** of the java web program. Here is a picture showing the scene. 

<p><img src="{{"assets/img/posts/2020-06-20-picdisposal-sec1.jpg" | relative_url}}" style="height: 30rem;"></p>

### Select a type of image processing
After designating IP and Port correctly, you will see a new surface containing colorful buttons and Images. In this section, what you need to do is just selecting a type of image processing and clicking on corresponding button. Here is an example where I select the image processing, **Nostalgia**. 

<p><img src="{{"assets/img/posts/2020-06-20-picdisposal-sec2.gif" | relative_url}}" style="height: 30rem;"></p>


### Fill, select, dispose, show and save

&emsp;The procedure of all image processing is similar. There are 5 steps in the procedure. 

- Firstly, fill out necessary columns. There are some columns in the section, such as Name, Clusters, Look-up table and so on. You should fill out these columns. 
- Secondly, click on **Select** button. After clicking on the button, you can select the picture you want to process. 
- Thirdly, click on **Dispose**. By clicking on the button, you will upload selected image to the server and require server to process selected image. 
- Fourthly, click on **Show** button. By clicking on **Show** button, treated image will be shown in current scene. 
- Fifthly, click on **Save** button. By clicking on **Save** button, you can obtain and store treated image. 

&emsp;Here is an example where I process an image with **Nostalgia**.

<p><img src="{{"assets/img/posts/2020-06-20-picdisposal-sec3.gif" | relative_url}}" style="height: 30rem;"></p>


# PicDisposal_py

## Intro

&emsp;Here is a python project containing several types of image image disposals. With the assistance of click, we can use command line to run specific image disposal. 

## Command Line

&emsp;If you want to figure out how to run with command line, open your terminal, move current path to the root of this project, and then type command line `python cmd.py --help` to  know the commands. Assuming that you want to know the structure of the command `binarize`, you can type command line, `python cmd.py binarize --help`, to know its structure.



# ImageDisposal

## Intro

&emsp;This is a javaweb project used for dealing with some affairs about android application, **PicDisposal**. If you run this javaweb project, your computer can be regarded as a server. Via network communication between your computer and android application, your computer can cope with various types of image disposals.  

## Note

&emsp;Before you run the server, you should determine two parameters in `com\zzwarn\options\CmdRunner.java`, **py_interpreter_loc** and **py_project_cmd_py_loc**.  **py_interpreter_loc** corresponds to the absolute path of python interpreter. **py_project_cmd_py_loc** corresponds to the absolute path of `cmd.py  ` which is a python file of the python project, [./PicDisposal_py](https://github.com/ZZwarn1998/PicDisposal/tree/master/PicDisposal_py). For example, the path of my python interpreter is `D:\\Anaconda3\\envs\\projenv\\python.exe`  and the path of `cmd.py` is `D:\\PCproj\\PicDisposal_py\\cmd.py`, therefore, we assign **py_interpreter_loc** `D:\\Anaconda3\\envs\\projenv\\python.exe` and   **py_project_cmd_py_loc** `D:\\PCproj\\PicDisposal_py\\cmd.py`.




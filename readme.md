Benefits of motion detector
  -alarm of burglar
  -exact time data when motion is detected whenever change in the frame of captured or live recording
  -saves money costs by switching off electric appliances
  -security and defence
  -surveillance

libraries and packages used:
  -pandas
  -numpy
  -cv2
  -bokeh
  -Jupyter

  pandas
    it is a easy to use data structure and data analysis tool for Python.
    in this project it is used for holding frame values in RGB format. in numPY array structure i.e. 2D array

  numPY
    Numpy is the core library for scientific computing in Python.
    It provides a high-performance multidimensional array object, and tools for working with these arrays.
    It efficiently stores image's rgb values.

  bokeh
    Bokeh is an interactive visualization library that targets modern web browsers for presentation.
    Its goal is to provide elegant, concise construction of versatile graphics, and to extend this capability with high-performance interactivity over very large or streaming datasets.
    Bokeh can help anyone who would like to quickly and easily create interactive plots, dashboards, and data applications.
    It is used for data visualization of timestamp of motion detection.

  cv2
	OpenCV-Python is a library of Python bindings designed to solve computer vision problems.
	It is used for comparing two frames for motion detection by comparing the two variable frame data.
	OpenCV-Python makes use of Numpy, which is a highly optimized library for numerical operations.

  Jupyter Notebook
    hybrid between interactive shell and editor!
    saves code ad test codes
    we use jupiter when we have lots of data processing
    in this porject it is used for processing data of the time of motion detection in and out time
    it can be used for crud operation of provided datasets


  process of execution of project
    when run!
    opens webcam [normal color]
    normal streaming converted into grayscale
    grayscale is blurred[gaussian] resulting into the translucent view similar to xray view also named as DELTA
    delta frame is conerted into pure black and white

    opencv is used for motion detetion > that compares first_frame value of RGB variable with current
    if it detects slight motion contour is formed.  [green rectangles]
    contour is also used for the face detection.

    if current frame and initial frame data are same! it is idle state [i.e. when there is no motion]
    this step of acquiring time data continues until program is closed


    when prrogram is closed!
    all the time data are saved in a file  with .csv format

      data can also be viewed in excel


    -------------------------------------------
    future works

    graph figures are shown with the help of bokeh package
    graph is made for the time in and time out of external object that results motion detection

    output file - graph.html is generated by the bokeh package automatically
	
    

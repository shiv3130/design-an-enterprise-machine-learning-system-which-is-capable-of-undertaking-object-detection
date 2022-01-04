# design-an-enterprise-machine-learning-system-which-is-capable-of-undertaking-object-detection
to design an enterprise machine learning system  which  is  capable  of  undertaking  object  detection  tasks.  In  this  coursework  you  are  required  to  implement your solution using Flask for your frontend application and allow it to communicate with  TensorFlow serving hosted in Docker using an appropriate communications protocol. The inferencing  elements of the system should be run on the GPU to provide appropriate inferencing speed.
Detail of the tasks
1) Development of the Flask web application
In  this  task,  you  are  required  to  develop  a  Flask  website  where  users  can  upload  images  for 
classification and view the results. Your site should target the current version of the Google Chrome 
web browser. The following tasks should be undertaken:
 The development of a theme for your site this includes design elements such as colour, font 
and spacing etc.
 You  should  endeavour  to  make  your  site  as  professionally  styled  as  you  can;  this  means 
using external style sheets wherever possible and only using internal style sheets for page 
specific styling (you should avoid using inline styling).
 You should create a home page called index.html that allows users to upload images using 
a form. Image uploads should be restricted to the following extensions (.jpg .jpeg .png) and 
should display a message if the user attempts to upload an invalid extension.
 You  should  develop  a  results  page  called  results.html  which  displays  the  classified  image 
(with bounding boxes) along with a table containing the image name, objects detected and 
associated probability. The results.html page should also display the original non-classified 
image so the user can compare the results.
2) Development of the Flask backend
In this task, you are required to develop the backend python code that will host your dynamic flask 
application.  All  of  your  code  should  be  fully  commented  and  produce  a  functional  flask  site.  Your 
code will need to enable the following:
 Images  submitted  from  the  form  on  the  index.html  page  should  be  processed  by  the 
TensorFlow serving framework using REST or gRPC. The original unclassified image should 
also be saved in a directory called originals in the root of your flask application.

 Functions for each of the pages (index.html and resutls.html) should also be generated so 
that the flask application can render the page with the required elements outlined in the first 
task.
 The  communication  stubs  should  be  implemented  to  support  either  the  REST  or  gRPC 
protocols.
 You will need to include all of the pessary code to produce a fully working Flask application 
which can be locally hosted on the Flask web development server.
3) TensorFlow serving and containerisation 
In this task you are required to productionise your Flask Object Detection application developed in 
task 1 and 2 using Docker. You will need to undertake the following:
 You are required to host your chosen TensorFlow model zoo model using the TensorFlow 
Serving  docker  image  with  GPU  support.  You  will  need  to  create  both  your  directory  and 
network mappings when calling the docker run command.
 You are required to create a docker file to move your application developed in task 1 and 2 
into a docker container. 
 You will need to build your new docker image and run it in docker. Both your Flask application 
and model hosted in TensorFlow serving should run within Docker.

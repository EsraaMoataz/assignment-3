# assignment-3

Problem :

Draw triangle with GLFW

-By using GLFW that enabled me to draw a multi color triangle with multi shader that :



-creating a window by using function
  {glfwCreateWindow}
  
- Check if the window is created or not ,if doesn't created output "Failed to create GLFW window" and terminate.

- load all OpenGL function pointers using function {gladLoadGLLoader}.

- Build and compile my shader program .

- Using function {glCreateShader} to create shader.

- create vertex shader "glCreateShader(GL_VERTEX_SHADER);".

- Check for shader compile errors by using function "glGetShaderiv(vertexShader, GL_COMPILE_STATUS, &success);"

- If compile error of vertex shader doesn't success then call the function "glGetShaderInfoLog" and output message "error".

- create fragment shader "glCreateShader(GL_FRAGMENT_SHADER);".

- Again,Check for shader compile errors by using function "glGetShaderiv(fragmentShader, GL_COMPILE_STATUS, &success);".

- Again,If compile error of fragment shader doesn't success then call the function "glGetShaderInfoLog" and output message "error".

- And then link between shaders by using function "glCreateProgram();" 

- then attach shaders using
       glAttachShader(shaderProgram, vertexShader);
       glAttachShader(shaderProgram, fragmentShader);
      
 - Check for linking errors using function "glGetProgramiv(shaderProgram, GL_LINK_STATUS, &success);"
 
 - finally delete shaders using function 
        glDeleteShader(vertexShader);
	glDeleteShader(fragmentShader);
         
	
	

	
	
	
	


	




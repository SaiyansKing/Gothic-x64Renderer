# Gothic x64Renderer  
This mod for the games Gothic and Gothic II brings the engine of those games into a more modern state. Through a custom implementation of the DirectDraw-API and using hooking and assembler-code-modifications of Gothic's internal engine calls, this mod completely replaces Gothic's old rendering architecture.  
  
The new renderer is able to utilize more of the current GPU generation's power. Since Gothic's engine in its original state tries to cull as much as possible, this takes a lot of work from the CPU, which was slowing down the game even on today's processors. While the original renderer did a really great job with the tech from 2002, GPUs have grown much faster.  
  
So how does it work? This modification works by proxifying rendering workflow onto 64bit process, which allows original Gothic process to not care about how much memory rendering scene will use.  
  
There are four graphic api available:  
- Vulkan 1.0+(Required extension: VK_KHR_maintenance1)  
- DirectX12  
- DirectX11  
- OpenGL 4.3+(Required extensions: GL_ARB_direct_state_access or GL_EXT_direct_state_access and GL_ARB_clip_control)  
  
## Special Thanks  
... to all people that worked on GD3D11 project.  
  
Release Date: somewhere in 31.12.2077  
  
If you like what I'm doing you can buy me coffee:  
https://ko-fi.com/saiyansking
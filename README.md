# Hypercube-Project
A Network Protocol for online XR functionality

Mission Statement: To create an open-source, decentralized protocol standard for 
online XR usage, and usage of XR applications within a browser, with game-like
speed. This protocol, (XR:// or HCTP://) will utilize existing API's like OpenXR
​by Khronos, and its very own markup language (HCML) to provide basic functionality
​to each Webspace (Equivalent of a Webpage), with extended functionality integrated
by the end-user. Hypercube aims to seamlessly integrate 3D VR rooms and AR
overlays into common web browsers such as Firefox or Chrome without much hassle.
If integration proves to be limiting, Hypercube would instead implement a
lightweight alternative itself until a solution is found. Hypercube also aims for
the Webspaces to be indexable by common or Hypercube-made browsers.

Specifications:
- Local Engine Environments (OpenGL or perhaps other/own implementation) specified
  by HCML through TCP at a low update speed with large packet sizes
- Dynamic Objects and Variables (OpenXR or perhaps own high speed implementation)
  specified by HCML through UDP at a high update speed with small packet sizes
- Integrates with standard HTTP/HTTPS sites, can display within as a passthrough
- AR Variables (OpenGL, OpenXR or other/own implementation) specified by HCML
  through TCP/UDP depending on the packet size and required update speed
- Aims to be suited for as low as 1mbps connections
- SHA Security and Password Encryption (HCTPS://, HCTPE://, XRS://, XRE://)
- HCML aims to be compatible with common languages such as C++ or Java for
  advanced Webspace development or game development. 

UX:
- Search for a Hypercube Webspace in a common browser (protocol is indexable)
- Open Webspace, Hypercube asks for a headset to be plugged in or worn, and if
  one is already being worn, or if accessing from a VR desktop or VR browser,
  Hypercube automatically enters the space.
- VR Webspaces work like in VRChat if a multiuser server is implemented. Single
  user pages work like small games.
- AR Webspaces are Overlays that implement passthrough or transparency, with
  2D and 3D elements, dynamic variables and environment recognition, and real
  world user tracking (non-infringing).
- Browser-based experience, without the lag or hard search for domains or
  server DNS addresses.

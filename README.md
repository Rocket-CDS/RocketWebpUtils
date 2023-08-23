# RocketWebpUtils

**NOTE: This project is not included int eh DNNrocket package.  While it is considered part of DNNrocket it uses it's own install package.**

RocketWebpUtils is a wrapper for the google unmanged assembly libwebp_x64.dll.  

On install the assembly will be locked if it has been used.  RocketWebpUtils has been created so it is not loaded on upgrade of DNNrocket.  

## Upgrading 
If the libwebp_x64.dll needs to be upgraded, this package can be used, the AppPool will need to be recycled and the RocketWebpUtils (Thumbnails) not used before installation, otherwise a lock will happen and the install will fail.

## Extra Assembly installation
**Some assemblies do not need to be upgraded often and to save upgrade processing they are installed by this package**  

### ThoughtWorks.QRCode.dll  
This package also installs ThoughtWorks.QRCode.dll.  
This is to reduce the size of the DNNrocket install package.  ThoughtWorks.QRCode.dll is fairly large and should not need upgrading often.

### 

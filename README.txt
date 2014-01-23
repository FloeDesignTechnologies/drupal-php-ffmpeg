PHP-FFmpeg
==========
This project is an API module that integrate with the PHP FFmpeg (https://github.com/PHP-FFMpeg/PHP-FFMpeg)
library. This module doesn't do anything by itself and is usually extended by
other projects that do something useful with FFmpeg.

Installation
------------

Follow the standard module installation guide (http://drupal.org/documentation/install/modules-themes/modules-7)
to install PHP FFmpeg. This module depends on the Composer Manager module (http://drupal.org/project/composer_manager),
so follow the instructions on its project page to install the third-party
libraries that this module requires.

Usage
-----
The module provides an administrative UI for the various configuration options
exposed by PHP FFmpeg library. To instantiate the PHP FFmpeg classes populated
with the configuration options, call $ffmpeg = php_ffmpeg(); or
$ffprobe = php_ffmpeg_probe in your module. Refer to the PHP FFmpeg library's
documentation for details on how to use the library.

Adapters are provided so the PHP FFmpeg library will uses Drupal for logging
and caching. The Monolog module (https://drupal.org/project/monolog)
is also supported as an alternative logging solution.
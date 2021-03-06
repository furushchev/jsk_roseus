^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package geneus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.1.26 (2014-11-10)
-------------------

1.1.25 (2014-10-10)
-------------------
* Do not generate message/service files which are already generated
* Merge remote-tracking branch 'refs/remotes/origin/master' into not-invoke-many-eus-when-genmsg
* Do not invoke many eus when generating ros message files

1.1.23 (2014-09-24)
-------------------
* Supress output from geneus if GENEUS_VERBOSE is not set to true
* Contributors: Ryohei Ueda

1.1.22 (2014-09-04)
-------------------
* remove more unused debug message
* remove unused debug message
* Contributors: Kei Okada

1.1.21 (2014-06-30)
-------------------
* cmake/roseus.cmake : do not compile roseus message if it couldnot find in find_package-ed
* Contributors: Kei Okada

1.1.20 (2014-06-29)
-------------------
* cmake/roseus.cmake : workaround for groovy, prevent overwrite catkin_LIBRARIES
* cmake/roseus.cmake : do not generate message for install package, since this component is not package_found-ed so far, try to run geneus next-time
* cmake/roseus.cmake : check if _depend_output is null string
* Contributors: Kei Okada

1.1.19 (2014-06-11)
-------------------

1.1.18 (2014-05-16)
-------------------
* previous commit does not work with multiple CMAKE_PREFIX_PATH
* do not compile if users already installed with roseus-msgs package
* Contributors: Kei Okada

1.1.17 (2014-05-11)
-------------------

1.1.16 (2014-05-11)
-------------------

1.1.15 (2014-05-10)
-------------------
* compile message even if not catkinized
* Contributors: Kei Okada

1.1.14 (2014-05-09)
-------------------
* geneus: add rospack_depends to find dependencies
* Contributors: Kei Okada

1.1.13 (2014-05-06)
-------------------

1.1.12 (2014-05-06)
-------------------
* check if rosbuild_init was called
* Contributors: Kei Okada

1.1.11 (2014-05-04)
-------------------

1.1.10 (2014-05-03)
-------------------

1.1.9 (2014-05-03)
------------------

1.1.8 (2014-05-02)
------------------

1.1.7 (2014-04-28)
------------------

1.1.6 (2014-04-28)
------------------

1.1.5 (2014-04-27)
------------------
* compile all dependent packages
* add target ALL to invoke compile
* Contributors: Kei Okada

1.1.4 (2014-04-25)
------------------
* use roseus_INSTALL_DIR variables so that we can put message file in different locate #68
* #63 seems introduce new bugs, reporeted on https://github.com/jsk-ros-pkg/jsk_visualization/pull/19
* Contributors: Kei Okada

1.1.3 (2014-04-14)
------------------
* fix for roseus message generation (`#51 <https://github.com/jsk-ros-pkg/jsk_roseus/issues/51>`_)
 * set _ROSBUILD_GENERATED_MSG_FILES null before rosbuild_get_msgs
 * check eus2 has executable permission in msg/srv generation on rosbuild
 * fix depend tag of geneus manifest.xml
 * check SOURCE_DIR before set generate_messages_py
 * add depends to generate_messages_to_py
* Contributors: Kei Okada, Ryohei Ueda

1.1.0 (2014-04-07)
------------------
* roseus.cmake: add depend to message_generation_py, use same code for both msg/srv generation
* generated_eus: do not write generated file if manifest.l is not exists
* add geneus package that generate ros message for euslisp
* Contributors: Kei Okada


Using Bio-Formats as a Java library
===================================

Bio-Formats as a Maven, Gradle or Ivy dependency
------------------------------------------------

All released :file:`.jar` artifacts are published to and can be obtained from
the `OME Artifactory <http://artifacts.openmicroscopy.org/artifactory>`_.  The
"Client Settings" section of the Artifactory main page provides example code
snippets for inclusion into your Gradle, Maven or Ivy project, which will
enable the use of this repository.

Examples of getting started with Bio-Formats using Maven or Gradle are given
in the https://github.com/openmicroscopy/bio-formats-examples repository.
`OMERO <http://github.com/openmicroscopy/openmicroscopy>`_ uses Ivy to manage
its Java dependencies including Bio-Formats.

.. note::
  In order to retrieve the NetCDF dependency of Bio-Formats, it is necessary
  to configure the Unidata releases repository in addition to Maven Central and
  the OME artifactory in your :examples:`pom.xml`, :examples:`build.gradle` or
  :file:`ivy.xml` file.

Bio-Formats as a Java library
-----------------------------

Alternatively Bio-Formats can be used by including its component jar files.
You can :downloads:`download formats-gpl.jar <artifacts/formats-gpl.jar>` to
use it as a library. Just add :file:`formats-gpl.jar` to your CLASSPATH or
build path. You will also need :file:`ome-common.jar` for common I/O functions,
:file:`ome-xml.jar` for metadata standardization, and
`SLF4J <https://www.slf4j.org/>`_ for :doc:`logging`.

Dependencies
^^^^^^^^^^^^

The complete list of current dependencies is as follows:

.. list-table::
    :header-rows: 1

    * - Package
      - Maven name
      - License
    * - `Logback Classic v1.1.1 <http://logback.qos.ch>`_
      - ch.qos.logback:logback-classic:1.1.1
      - `Eclipse Public License v1.0`_
    * - `Logback Core v1.1.1 <http://logback.qos.ch>`_
      - ch.qos.logback:logback-core:1.1.1
      - `Eclipse Public License v1.0`_
    * - `JHDF5 v14.12.0 <https://wiki-bsse.ethz.ch/display/JHDF5>`_
      - ch.systems.cisd:jhdf5:14.12.0
      - `Apache License v2.0`_
    * - `XMP Library for Java v5.1.2 <https://www.adobe.com/devnet/xmp.html>`_
      - com.adobe.xmp:xmpcore:5.1.2
      - `BSD License`_
    * - `JCommander v1.27 <http://jcommander.org/>`_
      - com.beust:jcommander:1.27
      - `Apache License v2.0`_
    * - `metadata-extractor v2.6.2 <https://github.com/drewnoakes/metadata-extractor>`_
      - com.drewnoakes:metadata-extractor:2.6.2
      - `Apache License v2.0`_
    * - `Kryo v2.24.0 <https://github.com/EsotericSoftware/kryo>`_
      - com.esotericsoftware.kryo:kryo:2.24.0
      - `BSD License`_
    * - `MinLog v1.2 <https://github.com/EsotericSoftware/minlog>`_
      - com.esotericsoftware.minlog:minlog:1.2
      - `BSD License`_
    * - `Guava v17.0 <https://github.com/google/guava>`_
      - com.google.guava:guava:17.0
      - `Apache License v2.0`_
    * - `JGoodies Common v1.7.0 <http://www.jgoodies.com/downloads/libraries/>`_
      - com.jgoodies:jgoodies-common:1.7.0
      - `BSD License`_
    * - `JGoodies Forms v1.7.2 <http://www.jgoodies.com/downloads/libraries/>`_
      - com.jgoodies:jgoodies-forms:1.7.2
      - `BSD License`_
    * - `Commons Collections v3.2.1 <http://commons.apache.org/collections/>`_
      - commons-collections:commons-collections:3.2.1
      - `Apache License v2.0`_
    * - `Commons Lang v2.4 <http://commons.apache.org/lang/>`_
      - commons-lang:commons-lang:2.4
      - `Apache License v2.0`_
    * - `Commons Logging v1.1.1 <http://commons.apache.org/logging/>`_
      - commons-logging:commons-logging:1.1.1
      - `Apache License v2.0`_
    * - `NetCDF-Java Library v4.3.22 <https://www.unidata.ucar.edu/software/thredds/current/netcdf-java/documentation.htm>`_
      - edu.ucar:netcdf:4.3.22
      - `MIT-Style License`_
    * - `Joda time v2.2 <https://github.com/JodaOrg/joda-time>`_
      - joda-time:joda-time:2.2
      - `Apache License v2.0`_
    * - `JUnit v4.10 <http://junit.org>`_
      - junit:junit:4.10
      - `Common Public License v1.0`_
    * - `Apache Log4j v1.2.17 <http://logging.apache.org/log4j/1.2>`_
      - log4j:log4j:1.2.17
      - `Apache License v2.0`_
    * - `ImageJ v1.48s <http://imagej.net/Welcome>`_
      - net.imagej:ij:1.48s
      - Public domain
    * - `Assume NG v1.2.4 <https://github.com/hierynomus/assumeng>`_
      - nl.javadude.assumeng:assumeng:1.2.4
      - `Apache License v2.0`_
    * - `Apache Velocity v1.6.4 <http://velocity.apache.org>`_
      - org.apache.velocity:velocity:1.6.4
      - `Apache License v2.0`_
    * - `BeanShell v2.0b4 <http://www.beanshell.org>`_
      - org.beanshell:bsh:2.0b4
      - `Sun Public License / LGPL`_
    * - `Hamcrest Core v1.1 <https://github.com/hamcrest/JavaHamcrest>`_
      - org.hamcrest:hamcrest-core:1.1
      - `BSD 3-Clause`_
    * - `Objenesis v2.1 <http://objenesis.org>`_
      - org.objenesis:objenesis:2.1
      - `Apache License v2.0`_
    * - `Perf4J v0.9.13 <https://github.com/perf4j/perf4j>`_
      - org.perf4j:perf4j:0.9.13
      - `Apache License v2.0`_
    * - `Native Library Loader v2.1.4 <https://github.com/scijava/native-lib-loader>`_
      - org.scijava:native-lib-loader:2.1.4
      - `BSD License`_
    * - `SLF4J API v1.7.4 <https://www.slf4j.org>`_
      - org.slf4j:slf4j-api:1.7.6
      - `MIT License`_
    * - `SLF4J LOG4J-12 Binding v1.7.6 <https://www.slf4j.org>`_
      - org.slf4j:slf4j-log4j12:1.7.6
      - `MIT License`_
    * - `TestNG v6.8 <http://testng.org/doc/>`_
      - org.testng:testng:6.8
      - `Apache License v2.0`_
    * - `SnakeYAML v1.6 <https://bitbucket.org/asomov/snakeyaml>`_
      - org.yaml:snakeyaml:1.6
      - `Apache License v2.0`_
    * - `Jakarta ORO v2.0.8 <http://jakarta.apache.org/oro>`_
      - oro:oro:2.0.8
      - `Apache License v2.0`_
    * - `Woolz v1.4.0 <http://www.emouseatlas.org/emap/analysis_tools_resources/software/woolz.html>`_
      - woolz:JWlz:1.4.0
      - `GPL v2`_
    * - `Xalan Java Serializer v2.7.2 <http://xml.apache.org/xalan-j>`_
      - xalan:serializer:2.7.2
      - `Apache License v2.0`_
    * - `Xalan Java v2.7.2 <http://xml.apache.org/xalan-j>`_
      - xalan:xalan:2.7.2
      - `Apache License v2.0`_
    * - `Xerces2 Java Parser v2.8.1 <http://xerces.apache.org/xerces2-j>`_
      - xerces:xercesImpl:2.8.1
      - `Apache License v2.0`_
    * - `XML Commons External Components XML APIs v1.3.04 <http://xerces.apache.org/xml-commons/components/external/>`_
      - xml-apis:xml-apis:1.3.04
      - `Apache License v2.0`_

As described in :ref:`versioning-policy`, the minor version number of a
Bio-Formats release will always be increased if the version of a
non-OME/external dependency is bumped.


.. _Apache License v2.0: https://spdx.org/licenses/Apache-2.0.html
.. _MIT License: https://spdx.org/licenses/MIT.html
.. _BSD 3-Clause: https://spdx.org/licenses/BSD-3-Clause.html
.. _Sun Public License / LGPL: http://www.beanshell.org/license.html
.. _Common Public License v1.0: https://spdx.org/licenses/CPL-1.0.html
.. _MIT-Style License: https://github.com/Unidata/thredds/blob/v4.3.22/cdm/license.txt
.. _BSD License: https://spdx.org/licenses/BSD-2-Clause.html
.. _Eclipse Public License v1.0: https://spdx.org/licenses/EPL-1.0.html
.. _GPL v2: https://spdx.org/licenses/GPL-2.0.html


Examples of usage
-----------------

File reading and performance:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

:source:`MultiFileExample <components/formats-gpl/utils/MultiFileExample.java>` -
Simple example of how to open multiple files simultaneously.

:source:`ParallelRead <components/formats-gpl/utils/ParallelRead.java>` -
Reads all files in given directory in parallel, using a separate thread for each.

:doc:`ReadWriteInMemory <in-memory>` -
Tests the Bio-Formats I/O logic to and from byte arrays in memory.

File writing:
^^^^^^^^^^^^^

:source:`MinimumWriter <components/formats-gpl/utils/MinimumWriter.java>` -
A command line utility demonstrating the minimum amount of metadata needed to
write a file.

:source:`TiledExport <components/formats-gpl/utils/TiledExportExample.java>` -
Shows how to convert a file one tile at a time, instead of one plane at a time (needed for very large images).

File compression:
^^^^^^^^^^^^^^^^^

:source:`makeLZW <components/formats-gpl/utils/MakeLZW.java>` -
Converts the given image file to an LZW-compressed TIFF.

Metadata extract/print:
^^^^^^^^^^^^^^^^^^^^^^^

:source:`GetPhysicalMetadata <components/formats-gpl/utils/GetPhysicalMetadata.java>` -
Uses Bio-Formats to extract some basic standardized (format-independent) metadata.

:source:`ImageInfo <components/bio-formats-tools/src/loci/formats/tools/ImageInfo.java>` -
A more involved command line utility for thoroughly reading an input file,
printing some information about it, and displaying the pixels
onscreen using the Bio-Formats viewer.

:source:`PrintTimestamps <components/formats-gpl/utils/PrintTimestamps.java>` -
A command line example demonstrating how to extract timestamps from a file.

:source:`PrintLensNA <components/formats-gpl/utils/PrintLensNA.java>` -
Uses Bio-Formats to extract lens numerical aperture in a format-independent manner from a dataset.

:source:`PrintROIs <components/formats-gpl/utils/PrintROIs.java>` -
A simple example of how to retrieve ROI data parsed from a file.

:source:`SubResolutionExample <components/formats-gpl/utils/SubResolutionExample.java>` -
Demonstration of the sub-resolution API.

Metadata add/edit:
^^^^^^^^^^^^^^^^^^

:source:`EditImageName <components/formats-gpl/utils/EditImageName.java>` -
Edits the given file's image name (but does not save back to disk).

:source:`EditTiffComment <components/formats-gpl/utils/EditTiffComment.java>` -
Allows raw user TIFF comment editing for the given TIFF files.

:source:`writeMapAnnotations <components/formats-gpl/utils/writeMapAnnotationsExample.java>` -
Example method to write MapAnnotations to the ome-xml.

:source:`CommentSurgery <components/formats-gpl/utils/CommentSurgery.java>` -
Edits a TIFF ImageDescription comment, particularly the OME-XML comment found in OME-TIFF files.

Image converters:
^^^^^^^^^^^^^^^^^

:source:`ImageConverter <components/bio-formats-tools/src/loci/formats/tools/ImageConverter.java>` -
A simple command line tool for converting between formats.

:source:`ConvertToOmeTiff <components/formats-gpl/utils/ConvertToOmeTiff.java>` -
Converts the given files to OME-TIFF format.

:source:`WritePreCompressedPlanes <components/formats-gpl/utils/WritePrecompressedPlanes.java>` -
Writes the pixels from a set of JPEG files to a single TIFF. The pixel data is used as-is, 
so no decompression or re-compression is performed.

ImageJ plugins:
^^^^^^^^^^^^^^^

:source:`Simple_Read <components/bio-formats-plugins/utils/Simple_Read.java>` -
A simple ImageJ plugin demonstrating how to use Bio-Formats to read files into
ImageJ (see :doc:`/users/imagej/index`).

:source:`Read_Image <components/bio-formats-plugins/utils/Read_Image.java>` -
An ImageJ plugin that uses Bio-Formats to build up an image stack, reading
image planes one by one (see :doc:`/users/imagej/index`).

:source:`Mass_Importer <components/bio-formats-plugins/utils/Mass_Importer.java>` -
A simple plugin for ImageJ that demonstrates how to open all image files in a
directory using Bio-Formats, grouping files with similar names to avoiding
opening the same dataset more than once (see :doc:`/users/imagej/index`).

Image processing utilities:
^^^^^^^^^^^^^^^^^^^^^^^^^^^

:source:`SewTiffs <components/formats-gpl/utils/SewTiffs.java>` -
Stitches the first plane from a collection of TIFFs into a single file.

:source:`SumPlanes <components/formats-gpl/utils/SumPlanes.java>` -
Sums together the image planes from the given file,and saves the result to a 16-bit TIFF.


A Note on Java Web Start (bioformats\_package.jar vs. formats-gpl.jar)
----------------------------------------------------------------------

To use Bio-Formats with your Java Web Start application, we recommend
using **formats-gpl.jar** rather than **bioformats\_package.jar**—the latter
is merely a bundle of **formats-gpl.jar** plus all its optional
dependencies.

The **bioformats\_package.jar** bundle is intended as a convenience (e.g. to
simplify installation as an ImageJ plugin), but is by no means the only
solution for developers. We recommend using **formats-gpl.jar** as a
separate entity depending on your needs as a developer.

The bundle is quite large because we have added support for several
formats that need large helper libraries (e.g. Imaris' HDF-based
format). However, these additional libraries are optional; Bio-Formats
has been coded using reflection so that it can both compile and run
without them.

When deploying a JNLP-based application, using **bioformats\_package.jar**
directly is not the best approach, since every time Bio-Formats is
updated, the server would need to feed another 15+ MB JAR file to the
client. Rather, Web Start is a case where you should keep the JARs
separate, since JNLP was designed to make management of JAR dependencies
trivial for the end user. By keeping **formats-gpl.jar** and the
optional dependencies separate, only a <1 MB JAR needs to be updated
when **formats-gpl.jar** changes.

As a developer, you have the option of packaging **formats-gpl.jar**
with as many or as few optional libraries as you wish, to cut down on
file size as needed. You are free to make whatever kind of "stripped
down" version you require. You could even build a custom
**formats-gpl.jar** that excludes certain classes, if you like.


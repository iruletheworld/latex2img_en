The Accelerated Guide
========================

This chapter aims to provide the necessary minimal processes for
conversion, so that the users can just jump in.

Before applying the procedures in this chapter, please make sure that
all the necessary software have been installed and all configurations
are complete.

Converting to SVG
--------------------

#. Copy the :code:`util` folder shipped with this tutorial to the
   directory of your TEX file.

#. Configure the TEX file's :code:`documentclass` as the following.

    .. literalinclude:: ../../demo_to_svg.tex
        :language: latex
        :lines: 4-11
        :linenos:

#. Use :code:`-shell-escape` to compile the TEX file. For example
   (replace the pointy brackets and the surrounded contents to your TEX
   file's filename),

    .. code-block:: bash

        xelatex -synctex=1 -interaction=nonstopmode -shell-escape <你TEX文件的文件名>.tex

#. The converted SVG files would be in the :code:`out_svg` folder.

Converting to PNG
----------------------

#. Copy the :code:`util` folder shipped with this tutorial to the
   directory of your TEX file.

#. Configure the TEX file's :code:`documentclass` as the following.

    .. literalinclude:: ../../demo_to_png.tex
        :language: latex
        :lines: 4-11
        :linenos:


#. Use :code:`-shell-escape` to compile the TEX file. For example
   (replace the pointy brackets and the surrounded contents to your TEX
   file's filename),

    .. code-block:: bash

        xelatex -synctex=1 -interaction=nonstopmode -shell-escape <你TEX文件的文件名>.tex

#. The converted SVG files would be in the :code:`out_png` folder.


Converting to EMF
--------------------

#. Copy the :code:`util` folder shipped with this tutorial to the
   directory of your TEX file.

#. Configure the TEX file's :code:`documentclass` as the following.

    .. literalinclude:: ../../demo_to_emf.tex
        :language: latex
        :lines: 4-24
        :linenos:

#. Use :code:`-shell-escape` to compile the TEX file. For example
   (replace the pointy brackets and the surrounded contents to your TEX
   file's filename),

    .. code-block:: bash

        xelatex -synctex=1 -interaction=nonstopmode -shell-escape <你TEX文件的文件名>.tex

#. The converted SVG files would be in the :code:`out_emf` folder.

Converting to EPS
----------------------

#. Copy the :code:`util` folder shipped with this tutorial to the
   directory of your TEX file.

#. Configure the TEX file's :code:`documentclass` as the following.

    .. literalinclude:: ../../demo_to_eps.tex
        :language: latex
        :lines: 4-25
        :linenos:

#. Use :code:`-shell-escape` to compile the TEX file. For example
   (replace the pointy brackets and the surrounded contents to your TEX
   file's filename),

    .. code-block:: bash

        xelatex -synctex=1 -interaction=nonstopmode -shell-escape <你TEX文件的文件名>.tex

#. The converted SVG files would be in the :code:`out_eps` folder.

For ease of debugging, in this chapter, the commands are divided into
different lines (combined as one line using :code:`&&`). These commands
can actually be placed in one single script, so that the settings of
:code:`documentclass` are simplified. Refer to :doc:`in_one_go` for details.

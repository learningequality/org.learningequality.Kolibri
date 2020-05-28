# Flatpak packaging for kolibri-installer-gnome

This package contains [Kolibri](https://learningequality.org/kolibri/) as well
as a GNOME front-end. To build and install this package on your system, use
flatpak-builder…

    flatpak-builder build-dir org.learningequality.Kolibri.yaml --install --user

Once it is installed, you can run Kolibri:

    flatpak run org.learningequality.Kolibri

Note that the Kolibri flatpak will use a different data directory than if it was
running on the host system. Instead of being located in ~/.kolibri, Kolibri's
database files will be stored in the Flatpak application's data directory, such
as `~/.var/app/org.learningequality.Kolibri/data/kolibri`. This can be changed
as usual by setting the `KOLIBRI_HOME` environment variable.


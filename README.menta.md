# pkg-mate-media (Menta Linux)

Debian packaging of mate-media 1.29.0 (from debian-mate-team/mate-media on Salsa,
1.26.2-1), switched to meson and built with `-Dwayland=yes -Din-process=true`
(upstream requires in-process for wayland). The volume control panel applet is
installed as the in-process library `libmate-volume-control-applet.so`
(`InProcess=true` in `org.mate.applets.GvcApplet.mate-panel-applet`).

Needs libmate-desktop >= 1.27.1 and libmate-panel-applet with in-process support
(mate-panel 1.29.x from pkg-mate-panel).

Versioning: `<upstream>-<debian rev>mentaN`; bump with `dch -i`.
CI builds on every push to `master`; tag `menta/<version>` also publishes a release.

@INTLTOOL_DESKTOP_RULE@
@INTLTOOL_DIRECTORY_RULE@

# .directory files used for the menus
directorydir=$(datadir)/desktop-directories
directory_in_files=				\
	Advanced.directory.in			\
	AllPrograms.directory.in		\
	Documentation.directory.in		\
	Edutainment.directory.in		\
	Root.directory.in			\
	Sawfish.directory.in			\
	ServerConfig.directory.in		\
	SystemConfig.directory.in		\
	Utilities.directory.in			\
	Accessories-More.directory.in		\
	Advanced-More.directory.in		\
	Desktop.directory.in			\
	Development-More.directory.in		\
	Documentation-More.directory.in		\
	Games-More.directory.in			\
	Graphics-More.directory.in		\
	Internet-More.directory.in		\
	Multimedia-More.directory.in		\
	Office-More.directory.in		\
	ServerConfig-More.directory.in		\
	Settings-More.directory.in		\
	SystemConfig-More.directory.in		\
	System-More.directory.in		\
	Utilities-More.directory.in

directory_DATA = $(directory_in_files:.directory.in=.directory)

# these are .desktop files that are symlinked to by other packages, 
# and replace the one that comes with the package. Bad hack.
overridedir=$(datadir)/desktop-menu-patches
override_in_files=				\
	gnome-accessibility.desktop.in		\
	gnome-pilot.desktop.in			\
	gnome-gdmsetup.desktop.in		\
	gthumb.desktop.in			\
	redhat-audio-player.desktop.in		\
	redhat-email.desktop.in			\
	redhat-evolution-mail.desktop.in		\
	redhat-evolution-calendar.desktop.in	\
	redhat-evolution-contacts.desktop.in	\
	redhat-evolution-tasks.desktop.in		\
	redhat-web.desktop.in			\
	redhat-diagrams.desktop.in		\
	redhat-drawing.desktop.in		\
	redhat-math.desktop.in			\
	redhat-presentations.desktop.in		\
	redhat-print.desktop.in			\
	redhat-spreadsheet.desktop.in		\
	redhat-word-processor.desktop.in	\
	openoffice-printeradmin.desktop.in	\
	openoffice-setup.desktop.in
override_DATA = $(override_in_files:.desktop.in=.desktop)

EXTRA_DIST= $(directory_in_files) $(override_in_files)
DISTCLEANFILES = $(directory_in_files:.directory.in=.directory) $(override_in_files:.desktop.in=.desktop)

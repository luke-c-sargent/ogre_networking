ACLOCAL_AMFLAGS= -I m4
noinst_HEADERS= BaseApplication.h

bin_PROGRAMS= OgreApp
OgreApp_SOURCES= BaseGui.cpp Ball.cpp BaseApplication.cpp Court.cpp Game.cpp GameObject.cpp Network.cpp Player.cpp Simulator.cpp SoundEffects.cpp Ball.h config.h Court.h Game.h GameObject.h Network.h OgreMotionState.h Player.h Simulator.h SoundEffects.h BaseGui.h

OgreApp_CPPFLAGS= -I$(top_srcdir)
OgreApp_CXXFLAGS=$(OGRE_CFLAGS) $(OIS_CFLAGS) $(bullet_CFLAGS) $(CEGUI_CFLAGS) $(CEGUI_OGRE_CFLAGS) $(sdl_CFLAGS)
OgreApp_LDADD= $(OGRE_LIBS) $(OIS_LIBS) $(bullet_LIBS) $(CEGUI_LIBS) $(CEGUI_OGRE_LIBS) $(sdl_LIBS)
OgreApp_LDFLAGS= -lOgreOverlay -lboost_system -lSDL_mixer

EXTRA_DIST= buildit makeit
AUTOMAKE_OPTIONS= foreign
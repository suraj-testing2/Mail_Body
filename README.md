filesystem-proposal-mods
========================

Boost Filesystem Library with modifications for the C++ standards committee proposal

To experiment (Windows):

  Export boost subversion repo, say to trunk-ex
  pushd trunk-ex
  delete boost/filesystem.hpp, boost/filesystem, libs/filesystem
  git clone git://github.com/Beman/filesystem-proposal-mods.git libs/filesystem
  pushd boost
  mklink filesystem.hpp ..\libs\filesystem\include\boost\filesystem.hpp
  mklink /d filesystem ..\libs\filesystem\include\boost\filesystem
  popd
  popd
  bootstrap
  b2
  
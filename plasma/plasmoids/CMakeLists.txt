add_subdirectory(src)

set(plasmoids
    git.github.scalgoon.panel
    io.gitgud.wackyideas.battery
    io.gitgud.wackyideas.digitalclocklite
    io.gitgud.wackyideas.win7showdesktop
    io.gitgud.wackyideas.networkmanagement
    io.gitgud.wackyideas.volume
    io.gitgud.wackyideas.keyboardlayout

    git.github.scalgoon.tenstart
    io.gitgud.wackyideas.SevenStart
    io.gitgud.wackyideas.seventasks
    io.gitgud.wackyideas.desktopcontainment
)

foreach(plasmoid IN LISTS plasmoids)
    plasma_install_package(${plasmoid} ${plasmoid})
endforeach()


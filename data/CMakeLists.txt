install (FILES "kdeconnect.contract" DESTINATION ${KDE_INSTALL_DATADIR}/contractor/)
install (FILES "kdeconnect-thunar.desktop" DESTINATION ${KDE_INSTALL_DATADIR}/Thunar/sendto/)
install(PROGRAMS org.kde.kdeconnect_open.desktop DESTINATION ${XDG_APPS_INSTALL_DIR})
install (FILES "kdeconnect-dde.desktop" DESTINATION ${KDE_INSTALL_DATADIR}/deepin/dde-file-manager/oem-menuextensions/)

if(NOT SAILFISHOS)
    install(FILES org.kde.kdeconnect.kcm.appdata.xml DESTINATION ${KDE_INSTALL_METAINFODIR})
endif()

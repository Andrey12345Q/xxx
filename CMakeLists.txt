include(PVS-Studio.cmake)
pvs_studio_add_target(TARGET ${PROJECT_NAME}.analyze ALL
                      OUTPUT
                      FORMAT errorfile
                      ANALYZE ${PROJECT_NAME}
                      MODE GA:1,2
                      LOG ${PROJECT_NAME}.log
                      ARGS -e C:/Qt/
                      HIDE_HELP)
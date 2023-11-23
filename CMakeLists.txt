if(NOT CMAKE_BUILD_EARLY_EXPANSION) 
        add_definitions(-DTABLESDIR "/spiffs/tables")
        add_definitions(-DENABLE_UCS4)
endif()

idf_component_register(SRCS "liblouis/commonTranslationFunctions.c"
                            "liblouis/compileTranslationTable.c"
                            "liblouis/logging.c"
                            "liblouis/lou_backTranslateString.c"
                            "liblouis/lou_translateString.c"
                            "liblouis/maketable.c"
                            "liblouis/metadata.c"
                            "liblouis/pattern.c"
                            "liblouis/utils.c"
                    INCLUDE_DIRS "liblouis")
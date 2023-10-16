add_definitions(-DTABLESDIR "/spiffs/tables")
add_definitions(-DENABLE_UCS4)

idf_component_register(SRCS "commonTranslationFunctions.c"
                            "compileTranslationTable.c"
                            "logging.c"
                            "lou_backTranslateString.c"
                            "lou_translateString.c"
                            "maketable.c"
                            "metadata.c"
                            "pattern.c"
                            "utils.c"
                    INCLUDE_DIRS "liblouis")
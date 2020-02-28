# Nous voulons un cmake "récent" pour utiliser les dernières fonctionnalités
cmake_minimum_required(VERSION 3.0)

# Notre projet est étiqueté hello
project(Borne)

# Crée des variables avec les fichiers à compiler
set(SRCS
    src/borne.cpp
    src/lecteurcarte.cpp

    )
    
set(HEADERS
    src/lcarte.h
    src/lecteurcarte.h
	src/memoire_borne.h
	src/donnees_borne.h
    )

# On indique que l'on veut un exécutable "Borne" compilé à partir des fichiers décrits par les variables SRCS et HEADERS
add_executable(Borne ${SRCS} ${HEADERS})
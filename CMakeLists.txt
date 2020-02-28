# Nous voulons un cmake "récent" pour utiliser les dernières fonctionnalités
cmake_minimum_required(VERSION 3.0)

# Notre projet est étiqueté hello
project(hello)

# Crée des variables avec les fichiers à compiler
set(SRCS
    borne.cpp
    lecteurcarte.cpp

    )
    
set(HEADERS
    lecteurcarte.h
	memoire_borne.h
	donnees_borne.h
    )

# On indique que l'on veut un exécutable "Borne" compilé à partir des fichiers décrits par les variables SRCS et HEADERS
add_executable(hello ${SRCS} ${HEADERS})
# javaPathHelper
OpenBSD java startup script helper

javaPathHelper is a script that java applications can use to provide a
consistent and familiar method for launching java applications on
OpenBSD. The use of JAVACMD, JAVA_HOME and PATH environment variables are
well known methods for users to control which JDK is used to launch a
java application.  When a user sets up thier environment javaPathHelper
will use it. No attempt is made to prevent the user from running an
application that requires a particular JDK version with a lower version.
When the user's environment has not be setup, javaPathHelper falls back
to inspecting which JDK satisfied the RUN_DEPENDS for the package.

# javadoc upload notes

the current build of swerve-docs links to our host of wpilib's javadocs. why? wpi's version of wpilib is hosted on http, hence you cannot link to it over the https connection that github.io provides.
because of this, wpilib's javadocs should be updated with new releases (usually one or two at the beginning of the season). to do this, you download the release source code from wpilibsuite from github.com/allwpilib, extract it, then run gradlew(.bat) eclipse, dump the contents of the wpilibj folder into a new eclipse project, then refresh eclipse, generate the javadoc, delete the old javadoc from your local version of the repository, then copy-paste the new one in.
 
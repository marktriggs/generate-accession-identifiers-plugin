To install, take a build of the ArchivesSpace master branch
(e.g. http://aspace.hudmol.com/build-snapshots/archivesspace.zip).
Then:

     unzip -x archivesspace.zip

     cd archivesspace/plugins
     git clone https://github.com/marktriggs/generate-accession-identifiers-plugin

     cd ../
     echo "AppConfig[:plugins] = ['generate-accession-identifiers-plugin']" > config/config.rb

     ./archivesspace.sh

Browsing to the "New Accession" form should generate an identifier
like `2013 000`.

Publish to local
----------------

While developing, you may need do local publish. Run
``sbt publish-local``.
Alternatively you can run ``sbt`` then from SBT command prompt run
``+ publish-local``.

To delete the local publish:

::

  $ find ~/.ivy2 -name *xitrum-scalatags* -delete

Publish to Sonatype
-------------------

See:
https://github.com/sbt/sbt.github.com/blob/gen-master/src/jekyll/using_sonatype.md

1. Copy content of
     dev/build.sbt.end   to the end of build.sbt
     dev/plugins.sbt.end to the end of project/plugins.sbt
2. Run ``sbt publish-signed``. Alternatively you can run ``sbt`` then from SBT
   command prompt run ``+ publish-signed``.
3. Login at https://oss.sonatype.org/ and from "Staging Repositories" select the
   newly published item, click "Close" then "Release".

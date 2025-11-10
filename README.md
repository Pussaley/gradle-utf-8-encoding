### Add the tasks below to solve UTF-8 problem in `Intellij IDEA`

>```code
>tasks.withType<JavaExec>().configureEach {
>    jvmArgs(
>        "-Dfile.encoding=UTF-8",
>        "-Dsun.stdout.encoding=UTF-8",
>        "-Dsun.stderr.encoding=UTF-8"
>    )
>}
>
>tasks.withType<JavaCompile>().configureEach {
>    options.encoding = "UTF-8"
>}
>```

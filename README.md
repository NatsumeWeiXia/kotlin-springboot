# kotlin-springboot
kotlin-Springboot test

test using maven kotlin to creat a springboot project

**worked but can not package**

error:


'''org.apache.maven.lifecycle.LifecycleExecutionException: Failed to execute goal org.jetbrains.kotlin:kotlin-maven-plugin:1.2.51:compile (default-cli) on project kotlin-springboot: Compilation failure
java.lang.IllegalStateException: The provided plugin org.jetbrains.kotlin.allopen.AllOpenComponentRegistrar is not compatible with this version of compiler
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:188)
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:120)
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment$Companion.createForProduction(KotlinCoreEnvironment.kt:433)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.createCoreEnvironment(K2JVMCompiler.kt:295)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.doExecute(K2JVMCompiler.kt:185)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.doExecute(K2JVMCompiler.kt:51)
	at org.jetbrains.kotlin.cli.common.CLICompiler.execImpl(CLICompiler.java:95)
	at org.jetbrains.kotlin.cli.common.CLICompiler.execImpl(CLICompiler.java:50)
	at org.jetbrains.kotlin.cli.common.CLITool.exec(CLITool.kt:88)
	at org.jetbrains.kotlin.maven.KotlinCompileMojoBase.execCompiler(KotlinCompileMojoBase.java:237)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execCompiler(K2JVMCompileMojo.java:237)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execCompiler(K2JVMCompileMojo.java:55)
	at org.jetbrains.kotlin.maven.KotlinCompileMojoBase.execute(KotlinCompileMojoBase.java:220)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execute(K2JVMCompileMojo.java:222)
	at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo(DefaultBuildPluginManager.java:134)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:207)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:153)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:145)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:116)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:80)
	at org.apache.maven.lifecycle.internal.builder.singlethreaded.SingleThreadedBuilder.build(SingleThreadedBuilder.java:51)
	at org.apache.maven.lifecycle.internal.LifecycleStarter.execute(LifecycleStarter.java:128)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:307)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:193)
	at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:106)
	at org.apache.maven.cli.MavenCli.execute(MavenCli.java:863)
	at org.apache.maven.cli.MavenCli.doMain(MavenCli.java:288)
	at org.apache.maven.cli.MavenCli.main(MavenCli.java:199)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced(Launcher.java:289)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launch(Launcher.java:229)
	at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode(Launcher.java:415)
	at org.codehaus.plexus.classworlds.launcher.Launcher.main(Launcher.java:356)
	at org.codehaus.classworlds.Launcher.main(Launcher.java:47)
Caused by: java.lang.AbstractMethodError: org.jetbrains.kotlin.allopen.AllOpenComponentRegistrar.registerProjectComponents(Lcom/intellij/mock/MockProject;Lorg/jetbrains/kotlin/config/CompilerConfiguration;)V
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:186)
	... 36 more


	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:212)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:153)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:145)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:116)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:80)
	at org.apache.maven.lifecycle.internal.builder.singlethreaded.SingleThreadedBuilder.build(SingleThreadedBuilder.java:51)
	at org.apache.maven.lifecycle.internal.LifecycleStarter.execute(LifecycleStarter.java:128)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:307)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:193)
	at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:106)
	at org.apache.maven.cli.MavenCli.execute(MavenCli.java:863)
	at org.apache.maven.cli.MavenCli.doMain(MavenCli.java:288)
	at org.apache.maven.cli.MavenCli.main(MavenCli.java:199)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced(Launcher.java:289)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launch(Launcher.java:229)
	at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode(Launcher.java:415)
	at org.codehaus.plexus.classworlds.launcher.Launcher.main(Launcher.java:356)
	at org.codehaus.classworlds.Launcher.main(Launcher.java:47)
Caused by: org.jetbrains.kotlin.maven.KotlinCompilationFailureException: Compilation failure
java.lang.IllegalStateException: The provided plugin org.jetbrains.kotlin.allopen.AllOpenComponentRegistrar is not compatible with this version of compiler
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:188)
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:120)
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment$Companion.createForProduction(KotlinCoreEnvironment.kt:433)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.createCoreEnvironment(K2JVMCompiler.kt:295)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.doExecute(K2JVMCompiler.kt:185)
	at org.jetbrains.kotlin.cli.jvm.K2JVMCompiler.doExecute(K2JVMCompiler.kt:51)
	at org.jetbrains.kotlin.cli.common.CLICompiler.execImpl(CLICompiler.java:95)
	at org.jetbrains.kotlin.cli.common.CLICompiler.execImpl(CLICompiler.java:50)
	at org.jetbrains.kotlin.cli.common.CLITool.exec(CLITool.kt:88)
	at org.jetbrains.kotlin.maven.KotlinCompileMojoBase.execCompiler(KotlinCompileMojoBase.java:237)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execCompiler(K2JVMCompileMojo.java:237)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execCompiler(K2JVMCompileMojo.java:55)
	at org.jetbrains.kotlin.maven.KotlinCompileMojoBase.execute(KotlinCompileMojoBase.java:220)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execute(K2JVMCompileMojo.java:222)
	at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo(DefaultBuildPluginManager.java:134)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:207)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:153)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:145)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:116)
	at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:80)
	at org.apache.maven.lifecycle.internal.builder.singlethreaded.SingleThreadedBuilder.build(SingleThreadedBuilder.java:51)
	at org.apache.maven.lifecycle.internal.LifecycleStarter.execute(LifecycleStarter.java:128)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:307)
	at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:193)
	at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:106)
	at org.apache.maven.cli.MavenCli.execute(MavenCli.java:863)
	at org.apache.maven.cli.MavenCli.doMain(MavenCli.java:288)
	at org.apache.maven.cli.MavenCli.main(MavenCli.java:199)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced(Launcher.java:289)
	at org.codehaus.plexus.classworlds.launcher.Launcher.launch(Launcher.java:229)
	at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode(Launcher.java:415)
	at org.codehaus.plexus.classworlds.launcher.Launcher.main(Launcher.java:356)
	at org.codehaus.classworlds.Launcher.main(Launcher.java:47)
Caused by: java.lang.AbstractMethodError: org.jetbrains.kotlin.allopen.AllOpenComponentRegistrar.registerProjectComponents(Lcom/intellij/mock/MockProject;Lorg/jetbrains/kotlin/config/CompilerConfiguration;)V
	at org.jetbrains.kotlin.cli.jvm.compiler.KotlinCoreEnvironment.<init>(KotlinCoreEnvironment.kt:186)
	... 36 more


	at org.jetbrains.kotlin.maven.MavenPluginLogMessageCollector.throwKotlinCompilerException(MavenPluginLogMessageCollector.java:111)
	at org.jetbrains.kotlin.maven.KotlinCompileMojoBase.execute(KotlinCompileMojoBase.java:223)
	at org.jetbrains.kotlin.maven.K2JVMCompileMojo.execute(K2JVMCompileMojo.java:222)
	at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo(DefaultBuildPluginManager.java:134)
	at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:207)
	... 21 more'''
  
  *Tried lots of solution on github/stackOverflow and so on , no one is working*

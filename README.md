[25Jun2024 15:20:52.229] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserver, --fml.forgeVersion, 47.3.1, --fml.mcVersion, 1.20.1, --fml.forgeGroup, net.minecraftforge, --fml.mcpVersion, 20230612.114412, nogui]
[25Jun2024 15:20:52.234] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher 10.0.9+10.0.9+main.dcd20f30 starting: java version 17.0.8 by Oracle Corporation; OS Linux arch amd64 version 5.15.0-70-generic
[25Jun2024 15:20:54.242] [main/INFO] [net.minecraftforge.fml.loading.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserver
[25Jun2024 15:20:54.266] [main/INFO] [gg.essential.loader.stage1.EssentialLoaderBase/]: Updating Essential Loader (stage2) version 1.6.2 (285f951adc7537f49ae3ef9fc0d2fd3e) from union:/home/mch/multicraft/servers/server379979/mods/essential_1-3-2-7_forge_1-20-1.jar%23288!/stage2_1-6-2_forge_1-17-1.jar
[25Jun2024 15:20:54.273] [main/FATAL] [cpw.mods.modlauncher.TransformationServicesHandler/MODLAUNCHER]: Encountered serious error loading transformation service, expect problems
java.util.ServiceConfigurationError: cpw.mods.modlauncher.api.ITransformationService: Provider gg.essential.container.loader.stage0.EssentialTransformationService could not be instantiated
	at java.util.ServiceLoader.fail(ServiceLoader.java:586) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.newInstance(ServiceLoader.java:813) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.get(ServiceLoader.java:729) ~[?:?]
	at cpw.mods.modlauncher.util.ServiceLoaderUtils.lambda$streamWithErrorHandling$0(ServiceLoaderUtils.java:39) ~[modlauncher-10.0.9.jar%2355!/:?]
	at java.util.stream.ReferencePipeline$3$1.accept(ReferencePipeline.java:197) ~[?:?]
	at java.util.ServiceLoader$ProviderSpliterator.tryAdvance(ServiceLoader.java:1499) ~[?:?]
	at java.util.Spliterator.forEachRemaining(Spliterator.java:332) ~[?:?]
	at java.util.stream.AbstractPipeline.copyInto(AbstractPipeline.java:509) ~[?:?]
	at java.util.stream.AbstractPipeline.wrapAndCopyInto(AbstractPipeline.java:499) ~[?:?]
	at java.util.stream.ReduceOps$ReduceOp.evaluateSequential(ReduceOps.java:921) ~[?:?]
	at java.util.stream.AbstractPipeline.evaluate(AbstractPipeline.java:234) ~[?:?]
	at java.util.stream.ReferencePipeline.collect(ReferencePipeline.java:682) ~[?:?]
	at cpw.mods.modlauncher.TransformationServicesHandler.discoverServices(TransformationServicesHandler.java:133) ~[modlauncher-10.0.9.jar%2355!/:?]
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:87) ~[modlauncher-10.0.9.jar%2355!/:?]
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:78) ~[modlauncher-10.0.9.jar%2355!/:?]
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) ~[modlauncher-10.0.9.jar%2355!/:?]
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) ~[modlauncher-10.0.9.jar%2355!/:?]
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) ~[bootstraplauncher-1.1.2.jar:?]
Caused by: java.lang.RuntimeException: java.lang.reflect.InvocationTargetException
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1OrThrow(EssentialTransformationServiceBase.java:27) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.lambda$new$0(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.util.DelegatingTransformationServiceBase.<init>(DelegatingTransformationServiceBase.java:13) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationService.<init>(EssentialTransformationService.java:7) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.newInstance(ServiceLoader.java:789) ~[?:?]
	... 16 more
Caused by: java.lang.reflect.InvocationTargetException
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1(EssentialTransformationServiceBase.java:47) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1OrThrow(EssentialTransformationServiceBase.java:25) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.lambda$new$0(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.util.DelegatingTransformationServiceBase.<init>(DelegatingTransformationServiceBase.java:13) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationService.<init>(EssentialTransformationService.java:7) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.newInstance(ServiceLoader.java:789) ~[?:?]
	... 16 more
Caused by: java.lang.NoClassDefFoundError: org/apache/commons/codec/digest/DigestUtils
	at gg.essential.loader.stage1.EssentialLoaderBase.getChecksum(EssentialLoaderBase.java:356) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.downloadFile(EssentialLoaderBase.java:473) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.doDownload(EssentialLoaderBase.java:326) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.load(EssentialLoaderBase.java:176) ~[?:?]
	at gg.essential.loader.stage1.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:46) ~[?:?]
	at gg.essential.loader.stage1.EssentialTransformationService.<init>(EssentialTransformationService.java:29) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1(EssentialTransformationServiceBase.java:47) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1OrThrow(EssentialTransformationServiceBase.java:25) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.lambda$new$0(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.util.DelegatingTransformationServiceBase.<init>(DelegatingTransformationServiceBase.java:13) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationService.<init>(EssentialTransformationService.java:7) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.newInstance(ServiceLoader.java:789) ~[?:?]
	... 16 more
Caused by: java.lang.ClassNotFoundException: org.apache.commons.codec.digest.DigestUtils
	at java.net.URLClassLoader.findClass(URLClassLoader.java:445) ~[?:?]
	at java.lang.ClassLoader.loadClass(ClassLoader.java:587) ~[?:?]
	at java.lang.ClassLoader.loadClass(ClassLoader.java:520) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.getChecksum(EssentialLoaderBase.java:356) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.downloadFile(EssentialLoaderBase.java:473) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.doDownload(EssentialLoaderBase.java:326) ~[?:?]
	at gg.essential.loader.stage1.EssentialLoaderBase.load(EssentialLoaderBase.java:176) ~[?:?]
	at gg.essential.loader.stage1.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:46) ~[?:?]
	at gg.essential.loader.stage1.EssentialTransformationService.<init>(EssentialTransformationService.java:29) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1(EssentialTransformationServiceBase.java:47) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.loadStage1OrThrow(EssentialTransformationServiceBase.java:25) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.lambda$new$0(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.util.DelegatingTransformationServiceBase.<init>(DelegatingTransformationServiceBase.java:13) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationServiceBase.<init>(EssentialTransformationServiceBase.java:20) ~[?:?]
	at gg.essential.container.loader.stage0.EssentialTransformationService.<init>(EssentialTransformationService.java:7) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:77) ~[?:?]
	at jdk.internal.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45) ~[?:?]
	at java.lang.reflect.Constructor.newInstanceWithCaller(Constructor.java:499) ~[?:?]
	at java.lang.reflect.Constructor.newInstance(Constructor.java:480) ~[?:?]
	at java.util.ServiceLoader$ProviderImpl.newInstance(ServiceLoader.java:789) ~[?:?]
	... 16 more
[25Jun2024 15:20:54.358] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.5 Source=union:/home/mch/multicraft/servers/server379979/libraries/org/spongepowered/mixin/0.8.5/mixin-0.8.5.jar%2365!/ Service=ModLauncher Env=SERVER
[25Jun2024 15:20:54.415] [main/INFO] [io.dogboy.serializationisbad.core.SerializationIsBad/]: Initializing SerializationIsBad, implementation type: modlauncher
[25Jun2024 15:20:54.859] [main/INFO] [io.dogboy.serializationisbad.core.SerializationIsBad/]: Using remote config file
[25Jun2024 15:20:54.860] [main/INFO] [io.dogboy.serializationisbad.core.SerializationIsBad/]: Loaded config file
[25Jun2024 15:20:54.860] [main/INFO] [io.dogboy.serializationisbad.core.SerializationIsBad/]:   Blocking Enabled: true
[25Jun2024 15:20:54.860] [main/INFO] [io.dogboy.serializationisbad.core.SerializationIsBad/]:   Loaded Patch Modules: 39
[25Jun2024 15:20:55.707] [main/WARN] [net.minecraftforge.fml.loading.moddiscovery.ModFileParser/LOADING]: Mod file /home/mch/multicraft/servers/server379979/libraries/net/minecraftforge/fmlcore/1.20.1-47.3.1/fmlcore-1.20.1-47.3.1.jar is missing mods.toml file
[25Jun2024 15:20:55.707] [main/WARN] [net.minecraftforge.fml.loading.moddiscovery.ModFileParser/LOADING]: Mod file /home/mch/multicraft/servers/server379979/libraries/net/minecraftforge/javafmllanguage/1.20.1-47.3.1/javafmllanguage-1.20.1-47.3.1.jar is missing mods.toml file
[25Jun2024 15:20:55.708] [main/WARN] [net.minecraftforge.fml.loading.moddiscovery.ModFileParser/LOADING]: Mod file /home/mch/multicraft/servers/server379979/libraries/net/minecraftforge/lowcodelanguage/1.20.1-47.3.1/lowcodelanguage-1.20.1-47.3.1.jar is missing mods.toml file
[25Jun2024 15:20:55.709] [main/WARN] [net.minecraftforge.fml.loading.moddiscovery.ModFileParser/LOADING]: Mod file /home/mch/multicraft/servers/server379979/libraries/net/minecraftforge/mclanguage/1.20.1-47.3.1/mclanguage-1.20.1-47.3.1.jar is missing mods.toml file
[25Jun2024 15:20:56.880] [main/WARN] [net.minecraftforge.jarjar.selection.JarSelector/]: Attempted to select two dependency jars from JarJar which have the same identification: Mod File:  and Mod File: . Using Mod File: 
[25Jun2024 15:20:56.883] [main/INFO] [net.minecraftforge.fml.loading.moddiscovery.JarInJarDependencyLocator/]: Found 45 dependencies adding them to mods collection


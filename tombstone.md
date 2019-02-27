```
2019-02-27 17:47:22.878 14982-14982/? E/appproc: ERROR: could not find class 'android.support.test.services.shellexecutor.ShellMain'
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534] JNI DETECTED ERROR IN APPLICATION: JNI NewGlobalRef called with pending exception java.lang.ClassNotFoundException: Didn't find class "android.support.test.services.shellexecutor.ShellMain" on path: DexPathList[[directory "."],nativeLibraryDirectories=[/system/lib, /vendor/lib, /system/lib, /vendor/lib]]
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   at java.lang.Class dalvik.system.BaseDexClassLoader.findClass(java.lang.String) (BaseDexClassLoader.java:125)
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String, boolean) (ClassLoader.java:379)
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String) (ClassLoader.java:312)
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534] 
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]     in call to NewGlobalRef
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534] "main" prio=5 tid=1 Runnable
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   | group="main" sCount=0 dsCount=0 flags=0 obj=0x12c01cd8 self=0xb2612000
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   | sysTid=14982 nice=0 cgrp=default sched=0/0 handle=0xb6f84514
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   | state=R schedstat=( 466838427 96021759 88 ) utm=39 stm=7 core=0 HZ=100
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   | stack=0xbf58a000-0xbf58c000 stackSize=8MB
2019-02-27 17:47:22.883 14982-14982/? A/app_process: java_vm_ext.cc:534]   | held mutexes= "mutator lock"(shared held)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #00 pc 0047eae1  /system/lib/libart.so (art::DumpNativeStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, int, BacktraceMap*, char const*, art::ArtMethod*, void*)+209)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #01 pc 0057c193  /system/lib/libart.so (art::Thread::DumpStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+355)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #02 pc 00577693  /system/lib/libart.so (art::Thread::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+83)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #03 pc 00395256  /system/lib/libart.so (art::JavaVMExt::JniAbort(char const*, char const*)+1254)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #04 pc 003956c1  /system/lib/libart.so (art::JavaVMExt::JniAbortV(char const*, char const*, char*)+113)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #05 pc 0014f207  /system/lib/libart.so (art::ScopedCheck::AbortF(char const*, ...)+71)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #06 pc 0014ed19  /system/lib/libart.so (art::ScopedCheck::CheckThread(_JNIEnv*)+457)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #07 pc 0014dc2c  /system/lib/libart.so (art::ScopedCheck::CheckPossibleHeapValue(art::ScopedObjectAccess&, char, art::JniValueType)+140)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #08 pc 0014cf85  /system/lib/libart.so (art::ScopedCheck::Check(art::ScopedObjectAccess&, bool, char const*, art::JniValueType*)+853)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #09 pc 0014ff1c  /system/lib/libart.so (art::CheckJNI::NewRef(char const*, _JNIEnv*, _jobject*, art::IndirectRefKind)+908)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #10 pc 001395e9  /system/lib/libart.so (art::CheckJNI::NewGlobalRef(_JNIEnv*, _jobject*)+41)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #11 pc 00002133  /system/bin/app_process32 (???)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #12 pc 0007825c  /system/lib/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+428)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #13 pc 00001db2  /system/bin/app_process32 (???)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #14 pc 000b69e4  /system/lib/libc.so (__libc_init+100)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #15 pc 000016cd  /system/bin/app_process32 (???)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   native: #16 pc 000016d8  /system/bin/app_process32 (???)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534]   (no managed stack frames)
2019-02-27 17:47:22.884 14982-14982/? A/app_process: java_vm_ext.cc:534] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] Runtime aborting...
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] Dumping all threads without appropriate locks held: thread list lock mutator lock
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] All threads:
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] DALVIK THREADS (6):
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "main" prio=5 tid=1 Runnable
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=0 dsCount=0 flags=0 obj=0x12c01cd8 self=0xb2612000
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14982 nice=0 cgrp=default sched=0/0 handle=0xb6f84514
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=R schedstat=( 476765557 98522047 93 ) utm=39 stm=8 core=0 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xbf58a000-0xbf58c000 stackSize=8MB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes= "abort lock" "mutator lock"(shared held)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 0047eae1  /system/lib/libart.so (art::DumpNativeStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, int, BacktraceMap*, char const*, art::ArtMethod*, void*)+209)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0057c193  /system/lib/libart.so (art::Thread::DumpStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+355)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00577693  /system/lib/libart.so (art::Thread::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+83)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 0059750e  /system/lib/libart.so (art::DumpCheckpoint::Run(art::Thread*)+1118)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0058e9f6  /system/lib/libart.so (art::ThreadList::RunCheckpoint(art::Closure*, art::Closure*)+534)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 0058e242  /system/lib/libart.so (art::ThreadList::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool)+882)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 0055f1b1  /system/lib/libart.so (art::AbortState::DumpAllThreads(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, art::Thread*) const+289)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 0055edd0  /system/lib/libart.so (art::AbortState::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&) const+176)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #08 pc 0054d366  /system/lib/libart.so (art::Runtime::Abort(char const*)+198)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #09 pc 0011fb23  /system/lib/libart.so (_ZNSt3__110__function6__funcIPFvPKcENS_9allocatorIS5_EES4_EclEOS3_+35)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #10 pc 0065f2eb  /system/lib/libart.so (android::base::LogMessage::~LogMessage()+1051)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #11 pc 0039550f  /system/lib/libart.so (art::JavaVMExt::JniAbort(char const*, char const*)+1951)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #12 pc 003956c1  /system/lib/libart.so (art::JavaVMExt::JniAbortV(char const*, char const*, char*)+113)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #13 pc 0014f207  /system/lib/libart.so (art::ScopedCheck::AbortF(char const*, ...)+71)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #14 pc 0014ed19  /system/lib/libart.so (art::ScopedCheck::CheckThread(_JNIEnv*)+457)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #15 pc 0014dc2c  /system/lib/libart.so (art::ScopedCheck::CheckPossibleHeapValue(art::ScopedObjectAccess&, char, art::JniValueType)+140)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #16 pc 0014cf85  /system/lib/libart.so (art::ScopedCheck::Check(art::ScopedObjectAccess&, bool, char const*, art::JniValueType*)+853)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #17 pc 0014ff1c  /system/lib/libart.so (art::CheckJNI::NewRef(char const*, _JNIEnv*, _jobject*, art::IndirectRefKind)+908)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #18 pc 001395e9  /system/lib/libart.so (art::CheckJNI::NewGlobalRef(_JNIEnv*, _jobject*)+41)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #19 pc 00002133  /system/bin/app_process32 (???)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #20 pc 0007825c  /system/lib/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+428)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #21 pc 00001db2  /system/bin/app_process32 (???)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #22 pc 000b69e4  /system/lib/libc.so (__libc_init+100)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #23 pc 000016cd  /system/bin/app_process32 (???)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #24 pc 000016d8  /system/bin/app_process32 (???)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   (no managed stack frames)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "Jit thread pool worker thread 0" prio=5 tid=2 Native
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c40030 self=0xa6b03000
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14985 nice=9 cgrp=default sched=0/0 handle=0xa6c84970
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 186687 850628 2 ) utm=0 stm=0 core=0 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa6b86000-0xa6b88000 stackSize=1022KB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait_queue_me+0xd0/0x116
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait+0xe2/0x1dd
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_futex+0x9b/0x70a
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_futex+0xaf/0xf6
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac2  [vdso] (__kernel_vsyscall+14)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0001edf8  /system/lib/libc.so (syscall+40)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00121df0  /system/lib/libart.so (art::ConditionVariable::WaitHoldingLocks(art::Thread*)+112)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00121d73  /system/lib/libart.so (art::ConditionVariable::Wait(art::Thread*)+35)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0059913a  /system/lib/libart.so (art::ThreadPool::GetTask(art::Thread*)+266)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 00598585  /system/lib/libart.so (art::ThreadPoolWorker::Run()+117)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 00597fbb  /system/lib/libart.so (art::ThreadPoolWorker::Callback(void*)+139)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 00071445  /system/lib/libc.so (__pthread_start(void*)+53)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #08 pc 000205db  /system/lib/libc.so (__start_thread+75)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #09 pc 0001ec16  /system/lib/libc.so (__bionic_clone+70)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   (no managed stack frames)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "Signal Catcher" prio=5 tid=3 WaitingInMainSignalCatcherLoop
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c80020 self=0xb2615c00
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14986 nice=0 cgrp=default sched=0/0 handle=0xa6aff970
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 346706 10093358 2 ) utm=0 stm=0 core=0 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa6a05000-0xa6a07000 stackSize=1006KB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_sigtimedwait+0xd7/0x19f
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_rt_sigtimedwait+0x6e/0x9c
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac4  [vdso] (__kernel_vsyscall+16)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 00074391  /system/lib/libc.so (__rt_sigtimedwait+33)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 0002abcc  /system/lib/libc.so (sigwait+76)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00568559  /system/lib/libart.so (art::SignalSet::Wait()+57)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 00567fea  /system/lib/libart.so (art::SignalCatcher::WaitForSignal(art::Thread*, art::SignalSet&)+250)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 005663cf  /system/lib/libart.so (art::SignalCatcher::Run(void*)+319)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 00071445  /system/lib/libc.so (__pthread_start(void*)+53)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 000205db  /system/lib/libc.so (__start_thread+75)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #08 pc 0001ec16  /system/lib/libc.so (__bionic_clone+70)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   (no managed stack frames)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "HeapTaskDaemon" prio=5 tid=4 Blocked
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c02988 self=0xb2613e00
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14990 nice=0 cgrp=default sched=0/0 handle=0xa66f3970
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 63159 2791709 1 ) utm=0 stm=0 core=1 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa65f1000-0xa65f3000 stackSize=1038KB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait_queue_me+0xd0/0x116
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait+0xe2/0x1dd
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_futex+0x9b/0x70a
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_futex+0xaf/0xf6
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac2  [vdso] (__kernel_vsyscall+14)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0001edf8  /system/lib/libc.so (syscall+40)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00121df0  /system/lib/libart.so (art::ConditionVariable::WaitHoldingLocks(art::Thread*)+112)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00121d73  /system/lib/libart.so (art::ConditionVariable::Wait(art::Thread*)+35)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 002cc495  /system/lib/libart.so (art::gc::TaskProcessor::GetTask(art::Thread*)+277)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 002ccee2  /system/lib/libart.so (art::gc::TaskProcessor::RunAllTasks(art::Thread*)+82)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 0048b757  /system/lib/libart.so (art::VMRuntime_runHeapTasks(_JNIEnv*, _jobject*)+55)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 001fd4f8  /system/framework/x86/boot-core-libart.oat (Java_dalvik_system_VMRuntime_runHeapTasks__+104)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at dalvik.system.VMRuntime.runHeapTasks(Native method)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   - waiting to lock an unknown object
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$HeapTaskDaemon.runInternal(Daemons.java:461)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$Daemon.run(Daemons.java:103)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.run(Thread.java:764)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "FinalizerWatchdogDaemon" prio=5 tid=5 Sleeping
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c028e8 self=0xb2613800
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14989 nice=0 cgrp=default sched=0/0 handle=0xa67f8970
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 40243 2890668 1 ) utm=0 stm=0 core=1 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa66f6000-0xa66f8000 stackSize=1038KB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait_queue_me+0xd0/0x116
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait+0xe2/0x1dd
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_futex+0x9b/0x70a
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_futex+0xaf/0xf6
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac4  [vdso] (__kernel_vsyscall+16)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0001edf8  /system/lib/libc.so (syscall+40)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 0012226d  /system/lib/libart.so (art::ConditionVariable::TimedWait(art::Thread*, long long, int)+157)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00479528  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, long long, int, bool, art::ThreadState)+664)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0047b1cd  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, art::mirror::Object*, long long, int, bool, art::ThreadState)+333)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 0049cd41  /system/lib/libart.so (art::Thread_sleep(_JNIEnv*, _jclass*, _jobject*, long long, int)+113)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 0001ed1a  /system/framework/x86/boot.oat (Java_java_lang_Thread_sleep__Ljava_lang_Object_2JI+202)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.sleep(Native method)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   - sleeping on <0x07557c2b> (a java.lang.Object)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.sleep(Thread.java:373)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   - locked <0x07557c2b> (a java.lang.Object)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.sleep(Thread.java:314)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$FinalizerWatchdogDaemon.sleepFor(Daemons.java:342)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$FinalizerWatchdogDaemon.waitForFinalization(Daemons.java:364)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:281)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$Daemon.run(Daemons.java:103)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.run(Thread.java:764)
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523] "FinalizerDaemon" prio=5 tid=6 Waiting
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c02848 self=0xb2613200
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14988 nice=0 cgrp=default sched=0/0 handle=0xa68fd970
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 45348 2964774 1 ) utm=0 stm=0 core=1 HZ=100
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa67fb000-0xa67fd000 stackSize=1038KB
2019-02-27 17:47:22.913 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait_queue_me+0xd0/0x116
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait+0xe2/0x1dd
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_futex+0x9b/0x70a
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_futex+0xaf/0xf6
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac2  [vdso] (__kernel_vsyscall+14)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0001edf8  /system/lib/libc.so (syscall+40)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00121df0  /system/lib/libart.so (art::ConditionVariable::WaitHoldingLocks(art::Thread*)+112)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00121d73  /system/lib/libart.so (art::ConditionVariable::Wait(art::Thread*)+35)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0047950c  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, long long, int, bool, art::ThreadState)+636)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 0047b1cd  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, art::mirror::Object*, long long, int, bool, art::ThreadState)+333)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 004953b5  /system/lib/libart.so (art::Object_waitJI(_JNIEnv*, _jobject*, long long, int)+85)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 00000a58  /system/framework/x86/boot.oat (Java_java_lang_Object_wait__JI+136)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Object.wait(Native method)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   - waiting on <0x0f7d2888> (a java.lang.Object)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Object.wait(Object.java:422)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:188)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   - locked <0x0f7d2888> (a java.lang.Object)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:209)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:232)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$Daemon.run(Daemons.java:103)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.run(Thread.java:764)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] "ReferenceQueueDaemon" prio=5 tid=7 Waiting
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=1 dsCount=0 flags=1 obj=0x12c02788 self=0xb2612c00
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14987 nice=0 cgrp=default sched=0/0 handle=0xa6a02970
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | state=S schedstat=( 98517 11001216 2 ) utm=0 stm=0 core=0 HZ=100
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xa6900000-0xa6902000 stackSize=1038KB
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes=
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait_queue_me+0xd0/0x116
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: futex_wait+0xe2/0x1dd
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: do_futex+0x9b/0x70a
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: SyS_futex+0xaf/0xf6
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   kernel: sysenter_after_call+0x0/0x10
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 00000ac2  [vdso] (__kernel_vsyscall+14)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0001edf8  /system/lib/libc.so (syscall+40)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00121df0  /system/lib/libart.so (art::ConditionVariable::WaitHoldingLocks(art::Thread*)+112)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 00121d73  /system/lib/libart.so (art::ConditionVariable::Wait(art::Thread*)+35)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0047950c  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, long long, int, bool, art::ThreadState)+636)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 0047b1cd  /system/lib/libart.so (art::Monitor::Wait(art::Thread*, art::mirror::Object*, long long, int, bool, art::ThreadState)+333)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 00495342  /system/lib/libart.so (art::Object_wait(_JNIEnv*, _jobject*)+82)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 000006a8  /system/framework/x86/boot.oat (Java_java_lang_Object_wait__+104)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Object.wait(Native method)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   - waiting on <0x0bd3e221> (a java.lang.Class<java.lang.ref.ReferenceQueue>)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:178)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   - locked <0x0bd3e221> (a java.lang.Class<java.lang.ref.ReferenceQueue>)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Daemons$Daemon.run(Daemons.java:103)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Thread.run(Thread.java:764)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] Aborting thread:
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] "main" prio=5 tid=1 Native
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | group="" sCount=0 dsCount=0 flags=0 obj=0x12c01cd8 self=0xb2612000
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | sysTid=14982 nice=0 cgrp=default sched=0/0 handle=0xb6f84514
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | state=R schedstat=( 493401159 98522047 105 ) utm=41 stm=8 core=0 HZ=100
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | stack=0xbf58a000-0xbf58c000 stackSize=8MB
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   | held mutexes= "abort lock"
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #00 pc 0047eae1  /system/lib/libart.so (art::DumpNativeStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, int, BacktraceMap*, char const*, art::ArtMethod*, void*)+209)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #01 pc 0057c193  /system/lib/libart.so (art::Thread::DumpStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+355)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #02 pc 00577693  /system/lib/libart.so (art::Thread::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+83)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #03 pc 0055f1f8  /system/lib/libart.so (art::AbortState::DumpThread(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, art::Thread*) const+56)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #04 pc 0055ef08  /system/lib/libart.so (art::AbortState::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&) const+488)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #05 pc 0054d366  /system/lib/libart.so (art::Runtime::Abort(char const*)+198)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #06 pc 0011fb23  /system/lib/libart.so (_ZNSt3__110__function6__funcIPFvPKcENS_9allocatorIS5_EES4_EclEOS3_+35)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #07 pc 0065f2eb  /system/lib/libart.so (android::base::LogMessage::~LogMessage()+1051)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #08 pc 0039550f  /system/lib/libart.so (art::JavaVMExt::JniAbort(char const*, char const*)+1951)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #09 pc 003956c1  /system/lib/libart.so (art::JavaVMExt::JniAbortV(char const*, char const*, char*)+113)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #10 pc 0014f207  /system/lib/libart.so (art::ScopedCheck::AbortF(char const*, ...)+71)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #11 pc 0014ed19  /system/lib/libart.so (art::ScopedCheck::CheckThread(_JNIEnv*)+457)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #12 pc 0014dc2c  /system/lib/libart.so (art::ScopedCheck::CheckPossibleHeapValue(art::ScopedObjectAccess&, char, art::JniValueType)+140)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #13 pc 0014cf85  /system/lib/libart.so (art::ScopedCheck::Check(art::ScopedObjectAccess&, bool, char const*, art::JniValueType*)+853)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #14 pc 0014ff1c  /system/lib/libart.so (art::CheckJNI::NewRef(char const*, _JNIEnv*, _jobject*, art::IndirectRefKind)+908)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #15 pc 001395e9  /system/lib/libart.so (art::CheckJNI::NewGlobalRef(_JNIEnv*, _jobject*)+41)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #16 pc 00002133  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #17 pc 0007825c  /system/lib/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+428)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #18 pc 00001db2  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #19 pc 000b69e4  /system/lib/libc.so (__libc_init+100)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #20 pc 000016cd  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   native: #21 pc 000016d8  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   (no managed stack frames)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] Pending exception java.lang.ClassNotFoundException: Didn't find class "android.support.test.services.shellexecutor.ShellMain" on path: DexPathList[[directory "."],nativeLibraryDirectories=[/system/lib, /vendor/lib, /system/lib, /vendor/lib]]
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Class dalvik.system.BaseDexClassLoader.findClass(java.lang.String) (BaseDexClassLoader.java:125)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String, boolean) (ClassLoader.java:379)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String) (ClassLoader.java:312)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:523] 
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531] JNI DETECTED ERROR IN APPLICATION: JNI NewGlobalRef called with pending exception java.lang.ClassNotFoundException: Didn't find class "android.support.test.services.shellexecutor.ShellMain" on path: DexPathList[[directory "."],nativeLibraryDirectories=[/system/lib, /vendor/lib, /system/lib, /vendor/lib]]
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   at java.lang.Class dalvik.system.BaseDexClassLoader.findClass(java.lang.String) (BaseDexClassLoader.java:125)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String, boolean) (ClassLoader.java:379)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   at java.lang.Class java.lang.ClassLoader.loadClass(java.lang.String) (ClassLoader.java:312)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531] 
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]     in call to NewGlobalRef
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531] "main" prio=5 tid=1 Runnable
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   | group="main" sCount=0 dsCount=0 flags=0 obj=0x12c01cd8 self=0xb2612000
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   | sysTid=14982 nice=0 cgrp=default sched=0/0 handle=0xb6f84514
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   | state=R schedstat=( 466838427 96021759 88 ) utm=39 stm=7 core=0 HZ=100
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   | stack=0xbf58a000-0xbf58c000 stackSize=8MB
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   | held mutexes= "mutator lock"(shared held)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #00 pc 0047eae1  /system/lib/libart.so (art::DumpNativeStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, int, BacktraceMap*, char const*, art::ArtMethod*, void*)+209)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #01 pc 0057c193  /system/lib/libart.so (art::Thread::DumpStack(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+355)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #02 pc 00577693  /system/lib/libart.so (art::Thread::Dump(std::__1::basic_ostream<char, std::__1::char_traits<char>>&, bool, BacktraceMap*, bool) const+83)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #03 pc 00395256  /system/lib/libart.so (art::JavaVMExt::JniAbort(char const*, char const*)+1254)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #04 pc 003956c1  /system/lib/libart.so (art::JavaVMExt::JniAbortV(char const*, char const*, char*)+113)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #05 pc 0014f207  /system/lib/libart.so (art::ScopedCheck::AbortF(char const*, ...)+71)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #06 pc 0014ed19  /system/lib/libart.so (art::ScopedCheck::CheckThread(_JNIEnv*)+457)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #07 pc 0014dc2c  /system/lib/libart.so (art::ScopedCheck::CheckPossibleHeapValue(art::ScopedObjectAccess&, char, art::JniValueType)+140)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #08 pc 0014cf85  /system/lib/libart.so (art::ScopedCheck::Check(art::ScopedObjectAccess&, bool, char const*, art::JniValueType*)+853)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #09 pc 0014ff1c  /system/lib/libart.so (art::CheckJNI::NewRef(char const*, _JNIEnv*, _jobject*, art::IndirectRefKind)+908)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #10 pc 001395e9  /system/lib/libart.so (art::CheckJNI::NewGlobalRef(_JNIEnv*, _jobject*)+41)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #11 pc 00002133  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #12 pc 0007825c  /system/lib/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+428)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #13 pc 00001db2  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #14 pc 000b69e4  /system/lib/libc.so (__libc_init+100)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #15 pc 000016cd  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   native: #16 pc 000016d8  /system/bin/app_process32 (???)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531]   (no managed stack frames)
2019-02-27 17:47:22.914 14982-14982/? A/app_process: runtime.cc:531] 
```
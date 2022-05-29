# 🎨 Awesome .Net Async [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

![Twitter URL](https://img.shields.io/badge/-@mehdi_hadeli-%231DA1F2?style=flat-square&logo=twitter&logoColor=ffffff) 
[![blog](https://img.shields.io/badge/blog-dotnetuniversity.com-brightgreen?style=flat-square)](https://dotnetuniversity.com/https://dotnetuniversity.com/)


> Curated list of awesome articles and resources to learning and practicing about async, threading, and channels in .Net platform. this repository will be updated continuously, keep yourself up to date 😉

Contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/mehdihadeli/awesome-dotnet-async/blob/master/contributing.md) pages first.

Thanks to all [contributors](https://github.com/mehdihadeli/awesome-dotnet-async/graphs/contributors), you're awesome and wouldn't be possible without you! The goal is to build a categorized community-driven collection of very well-known resources.

## Contents
- [Guideline](#guide-line)
- [Async And Await](#async-and-await)
- [Cancellation](#cancellation)
- [IO-Bound](#io-bound)
- [Cpu-Bound](#cpu-bound)
- [TaskCompletionSource](#taskcompletionsource)
- [Task](#task)
- [ValueTask](#valuetask)
- [Configure Await](#configure-await)
- [Exception Handling](#exception-handling)
- [SynchronizationContext](#synchronizationcontext)
- [Awaiter](#awaiter)
- [Continuations](#continuations)
- [Thread Pool](#thread-pool)
- [Thread](#thread)
- [Async Tips](#async-tips)
- [Concurrency Vs Parallelism](#concurrency-vs-parallelism)
- [Async Local](#async-local)
- [Thread Safey](#thread-safey)
- [Asynchronous Messaging](#asynchronous-messaging)
- [Async Collections](#async-collections)
- [Async Stream And IEnumerableAsync](#async-stream-and-ienumerableasync)
- [Lazy Initialization](#lazy-initialization)
- [Iterators](#iterators)
- [Channels](#channels)
- [Libraries](#libraries)
- [Code Analyzers](#code-analyzers)
- [Other Resources](#other-resources)

## Guideline 

- [David Folwer - Async guideline ](https://github.com/davidfowl/AspNetCoreDiagnosticScenarios/blob/master/AsyncGuidance.md)

## Async And Await

### 📝 Articles
- [Async Overview](https://docs.microsoft.com/en-us/dotnet/standard/async)
- [Asynchronous programming patterns](https://docs.microsoft.com/en-us/dotnet/standard/asynchronous-programming-patterns/)
- [Task-based asynchronous pattern - TAP](https://b2n.ir/143257)
- [Event-based Asynchronous Pattern - EAP](https://b2n.ir/604805)
- [Asynchronous Programming Model - APM](https://docs.microsoft.com/en-us/dotnet/standard/asynchronous-programming-patterns/asynchronous-programming-model-apm)
- [Task asynchronous programming model](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/task-asynchronous-programming-model)
- [Async return types (C#)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/async-return-types)
- [When to Use Async and Await and How it Works](https://hamidmosalla.com/2018/03/30/when-to-use-async-and-await-and-how-it-works/)
- [Asynchrony in C# 5 Part Six: Whither async?](https://docs.microsoft.com/en-us/archive/blogs/ericlippert/asynchrony-in-c-5-part-six-whither-async)
- [Exploring the async/await State Machine – Series Overview](https://vkontech.com/exploring-the-async-await-state-machine-series-overview/)
- [Exploring the async/await State Machine – The Awaitable Pattern](https://vkontech.com/exploring-the-async-await-state-machine-the-awaitable-pattern/)
- [Exploring the async/await State Machine – Main Workflow and State Transitions](https://vkontech.com/exploring-the-async-await-state-machine-main-workflow-and-state-transitions/)
- [Exploring the async/await State Machine – Conceptual Implementation](https://vkontech.com/exploring-the-async-await-state-machine-conceptual-implementation/)
- [Dissecting the async methods in C#](https://devblogs.microsoft.com/premier-developer/dissecting-the-async-methods-in-c/)
- [Extending the async methods in C#](https://devblogs.microsoft.com/premier-developer/extending-the-async-methods-in-c/)
- [Understanding async/await State Machine in .NET](https://mykkon.work/async-state-machine/)
- [Fixing the Sync over Async antipattern](https://makolyte.com/fixing-the-sync-over-async-antipattern/)
- [Parallel Programming BY examples](http://diranieh.com/NETCSharp/ParallelWithExamples.htm)
- [Async/Await FAQ](https://devblogs.microsoft.com/pfxteam/asyncawait-faq/)
- [Are deadlocks still possible with await?](https://devblogs.microsoft.com/pfxteam/are-deadlocks-still-possible-with-await/)
- [Explaining Async and Await in ASP.NET](https://exceptionnotfound.net/using-async-and-await-in-asp-net-what-do-these-keywords-mean/)
- [A Practical Example Of Asynchronous Programming in C# and ASP.NET](https://exceptionnotfound.net/asynchronous-programming-asp-net-csharp-practical-guide-refactoring/)
- [The Ultimate Guide to Async and Await in C# and ASP.NET](https://exceptionnotfound.net/async-await-in-asp-net-csharp-ultimate-guide/)
- [AsyncGuidance](https://github.com/davidfowl/AspNetCoreDiagnosticScenarios/blob/master/AsyncGuidance.md)
- [Async Await Best Practices](https://github.com/brminnick/AsyncAwaitBestPractices)

## Cancellation

### 📝 Articles
- [Task cancellation in C# and things you should know about it](https://binary-studio.com/2015/10/23/task-cancellation-in-c-and-things-you-should-know-about-it)
- [Cancel asynchronous operation in csharp](https://johnthiriet.com/cancel-asynchronous-operation-in-csharp/)
- [Aborting Thread Vs Cancelling Task](https://www.c-sharpcorner.com/article/aborting-thread-vs-cancelling-task/)
- [Task cancellation](https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/task-cancellation)
- [Cancellation in Managed Threads](https://docs.microsoft.com/en-us/dotnet/standard/threading/cancellation-in-managed-threads)
- [Destroying threads](https://docs.microsoft.com/en-us/dotnet/standard/threading/destroying-threads)
- [How to: Cancel a Task and Its Children](https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/how-to-cancel-a-task-and-its-children)
- [Using CancellationTokens in ASP.NET Core MVC controllers](https://andrewlock.net/using-cancellationtokens-in-asp-net-core-mvc-controllers/)
- [Canceling HTTP Requests in ASP.NET Core with CancellationToken](https://code-maze.com/canceling-http-requests-in-asp-net-core-with-cancellationtoken/)
### 🔖 Samples

- [https://github.com/johnthiriet/AsyncTips](https://github.com/johnthiriet/AsyncTips)


## IO-Bound

### 📝 Articles

- [Deeper Dive into Tasks for an I/O-Bound Operation](http://docs.microsoft.com/en-us/dotnet/standard/async-in-depth#deeper-dive-into-tasks-for-an-io-bound-operation)
- [I/O-bound tasks](http://docs.microsoft.com/en-us/dotnet/standard/asynchronous-programming-patterns/implementing-the-task-based-asynchronous-pattern#io-bound-tasks)
- [Why you should not create asynchronous wrappers with Task.Run()](https://www.ben-morris.com/why-you-shouldnt-create-asynchronous-wrappers-with-task-run/)
- [Asynchronous file access (C#)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/using-async-for-file-access)
- [C# : TASK PARALLEL LIBRARY (TPL) WITH ASYNC AWAIT AND TASKCOMPLETIONSOURCE FOR ASYNC I/O OPERATIONS](https://b2n.ir/686253)
- [There Is No Thread](https://blog.stephencleary.com/2013/11/there-is-no-thread.html)
- [Wrapping Other Asynchronous Patterns in Awaitable Tasks](http://www.damirscorner.com/blog/posts/20130722-WrappingOtherAsynchronousPatternsInAwaitableTasks.html)
- [Task.Factory.StartNew vs Task.Factory.FromAsync](https://stackoverflow.com/questions/17432306/task-factory-startnew-vs-task-factory-fromasync)
- [Task.Run vs Task.Factory.StartNew](https://devblogs.microsoft.com/pfxteam/task-run-vs-task-factory-startnew/)

## Cpu-Bound

### 📝 Articles
- [Compute-bound tasks](https://b2n.ir/481224)
- [Task.Run Etiquette and Proper Usage](https://blog.stephencleary.com/2013/10/taskrun-etiquette-and-proper-usage.html)
- [Should I expose asynchronous wrappers for synchronous methods?](https://devblogs.microsoft.com/pfxteam/should-i-expose-asynchronous-wrappers-for-synchronous-methods/)
- [Task.Run Vs TaskCompletionSource Vs Task.Factory.FromAsync](https://b2n.ir/489838)
- [Task.Run vs Task.Factory.StartNew](https://devblogs.microsoft.com/pfxteam/task-run-vs-task-factory-startnew/)

## TaskCompletionSource

### 📝 Articles
- [Should I expose asynchronous wrappers for synchronous methods?](https://b2n.ir/959223)
- [Using TaskCompletionSource to change the semantics of async calls](http://vannevel.net/posts/using-taskcompletionsource-to-change-the-semantics-of-async-calls/)
- [TaskCompletionSource in real life (part 1 of 2)](https://www.fmork.net/software/writing/2012/TaskCompletionSource-in-real-life-(part-1-of-2).htm)
- [TaskCompletionSource in real life (part 2 of 2)](https://www.fmork.net/software/writing/2012/TaskCompletionSource-in-real-life-(part-2-of-2).htm)
- [C# : TASK PARALLEL LIBRARY (TPL) WITH ASYNC AWAIT AND TASKCOMPLETIONSOURCE FOR ASYNC I/O OPERATIONS](https://www.techblogcity.com/2019/06/05/task-parallel-library-with-async-await-and-taskcompletionsource/)
- [Task.Run Vs TaskCompletionSource Vs Task.Factory.FromAsync](https://hamidmosalla.com/2018/05/27/task-run-vs-taskcompletionsource-vs-task-factory-fromasync/)
- [The Nature of TaskCompletionSource](https://devblogs.microsoft.com/pfxteam/the-nature-of-taskcompletionsourcetresult/) - Stephen Toub
- [When should TaskCompletionSourceT be used?](https://stackoverflow.com/questions/15316613/when-should-taskcompletionsourcet-be-used)
- [Instance of Task class (Task.Factory.StartNew or TaskCompletionSource)](https://stackoverflow.com/questions/5674895/instance-of-task-class-task-factory-startnew-or-taskcompletionsource)
- [Wrapping Other Asynchronous Patterns in Awaitable Tasks](https://b2n.ir/871581)
- [The danger of TaskCompletionSource class](https://devblogs.microsoft.com/premier-developer/the-danger-of-taskcompletionsourcet-class/)
- [Mechanisms for Creating Tasks](https://devblogs.microsoft.com/pfxteam/mechanisms-for-creating-tasks/)
## Task

### Articles
- [Mechanisms for Creating Tasks](https://devblogs.microsoft.com/pfxteam/mechanisms-for-creating-tasks/) - Stephen Toub
- [Task Class](https://docs.microsoft.com/en-us/dotnet/api/system.threading.tasks.task)
- [New Task APIs in .NET 4.6](https://devblogs.microsoft.com/pfxteam/new-task-apis-in-net-4-6/) - Stephen Toub
- [Tasks, Monads, and LINQ](https://devblogs.microsoft.com/pfxteam/tasks-monads-and-linq/) - Stephen Toub
- [Serial vs Parallel task execution](https://www.davidguida.net/serial-vs-parallel-task-execution/)
## ValueTask

### 📝 Articles

- [ValueTask Restrictions - Stephen Cleary](https://blog.stephencleary.com/2020/03/valuetask.html)
- [How to use ValueTask in C#](https://morioh.com/p/da3a36ccbe3b)
- [Task, Async Await, ValueTask, IValueTaskSource and how to keep your sanity in modern .NET world](https://blog.scooletz.com/2018/05/14/task-async-await-valuetask-ivaluetasksource-and-how-to-keep-your-sanity-in-modern-net-world/)
- [.NET 5 and pooling for ValueTasks - Scooletz](https://blog.scooletz.com/2020/06/01/pooling-for-value-tasks-in-net5)

### 📹 Videos
- [Understanding how to use Task and ValueTask](https://www.youtube.com/watch?v=fj-LVS8hqIE)
- [When to use ValueTask instead of Task and save precious memory in C#](https://www.youtube.com/watch?v=mEhkelf0K6g)
## Configure Await

### 📝 Articles

- [ConfigureAwait FAQ - Stephen Toub](https://devblogs.microsoft.com/dotnet/configureawait-faq/)


## Exception Handling

### 📝 Articles

- [Exception Handling In Asynchronous Code](https://b2n.ir/836643)
- [Exception Handling in C# Asynchronous Programming](https://www.c-sharpcorner.com/UploadFile/dacca2/asynchronous-programming-in-C-Sharp-5-0-part-4-exception-handlin/)
- [Exception handling (Task Parallel Library)](https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/exception-handling-task-parallel-library)
- [Asynchrony in C# 5, Part Seven: Exceptions](https://docs.microsoft.com/en-us/archive/blogs/ericlippert/asynchronous-programming-in-c-5-0-part-two-whence-await)
## SynchronizationContext

### 📝 Articles

- [What Is SynchronizationContext](https://hamidmosalla.com/2018/06/24/what-is-synchronizationcontext/)



## Awaiter

### 📝 Articles

- [A Tour of Task, Part 6: Results](https://blog.stephencleary.com/2014/12/a-tour-of-task-part-6-results.html)
- [Task.Wait() Vs Task.GetAwaiter().GetResult()](https://jaliyaudagedara.blogspot.com/2019/06/taskwait-vs-taskgetawaitergetresult.html)
- [Avoid GetAwaiter().GetResult() at all cost](https://gsferreira.com/archive/2020/08/avoid-getawaiter-getresult-at-all-cost/)
- [Understanding C# async / await (2) The Awaitable-Awaiter Pattern](https://weblogs.asp.net/dixin/understanding-c-sharp-async-await-2-awaitable-awaiter-pattern)



## Continuations

### 📝 Articles

- [A Tour of Task, Part 7: Continuations](https://blog.stephencleary.com/2015/01/a-tour-of-task-part-7-continuations.html)
- [Chaining tasks using continuation tasks](https://docs.microsoft.com/en-us/dotnet/standard/parallel-programming/chaining-tasks-by-using-continuation-tasks)


## Thread Pool



## Thread

### 📝 Articles
- [Multithreading Basics](http://diranieh.com/NETThreading/MultithreadingBasics.htm)

## Async Tips

### 📝 Articles
- [Async Guidance](https://github.com/davidfowl/AspNetCoreDiagnosticScenarios/blob/master/AsyncGuidance.md)
- [Async and Await: Here be dragons](https://gist.github.com/ghuntley/e5b5642ecc4428255e61185bb79856e4)
- [Top 7 Common Async Mistakes](https://hamidmosalla.com/2018/04/21/top-7-common-async-mistakes/)
- [Async/Await - Best Practices in Asynchronous Programming](https://docs.microsoft.com/en-us/archive/msdn-magazine/2013/march/async-await-best-practices-in-asynchronous-programming)
- [Common C# async and await misconceptions](https://saebamini.com/common-async-and-await-misconceptions/)
- [Cancel Asynchronous Operation In Csharp](https://b2n.ir/n06328) - John Thiriet
- [C# Async Tips and Tricks](https://cpratt.co/async-tips-tricks/) - Chris Pratt
- [Eliding Async and Await](https://blog.stephencleary.com/2016/12/eliding-async-await.html) - Stephen Cleary
- [Async code smells and how to track them down with analyzers - Part I](https://cezarypiatek.github.io/post/async-analyzers-p1/)
- [Async code smells and how to track them down with analyzers - Part II](https://cezarypiatek.github.io/post/async-analyzers-p2/)
- [Two Ways to Do Async/Await in ASP.NET Wrong (and How to Fix Them)](https://exceptionnotfound.net/two-ways-to-do-async-await-in-asp-net-wrong-and-how-to-fix-them/)
### Videos
- [Is awaiting a Task instead of returning it directly in C# actually slower?](https://www.youtube.com/watch?v=Q2zDatDVnO0)

### 🔖 Samples
- [https://github.com/davidfowl/AspNetCoreDiagnosticScenarios](https://github.com/davidfowl/AspNetCoreDiagnosticScenarios)
	> This repository has examples of broken patterns in ASP.NET Core applications

## Concurrency Vs Parallelism

### 📝 Articles

- [Concurrency Vs Parallelism](https://hamidmosalla.com/2018/03/16/concurrency-vs-parallelism/)
- [Concurrency, part 1: Parallelism, Asynchrony, and Multi-threading Explained](https://blog.slaks.net/2014-12-23/parallelism-async-threading-explained/)


## Async Local

### 📝 Articles
- [AsyncLocalT in .NET 4.6](https://www.tabsoverspaces.com/233526-asynclocal-t-in-net-46)
- [Implicit Async Context ("AsyncLocal")](https://blog.stephencleary.com/2013/04/implicit-async-context-asynclocal.html)
- [Multithreaded shared variables and AsyncLocal](https://programmer.help/blogs/multithreaded-shared-variables-and-asynclocal.html)

## Thread Safey

### 📝 Articles

- [Thread Safety](https://hamidmosalla.com/2018/07/09/thread-safety/)



## Asynchronous Messaging

### 📝 Articles

- [Asynchronous Messaging, Part 1: Basic Distributed Architecture](https://blog.stephencleary.com/2021/01/asynchronous-messaging-1-basic-distributed-architecture.html)
- [Asynchronous Messaging, Part 2: Durable Queues](https://blog.stephencleary.com/2021/01/asynchronous-messaging-2-durable-queues.html)
- [Asynchronous Messaging, Part 3: Backend Service](https://blog.stephencleary.com/2021/01/asynchronous-messaging-3-backend-processor.html)



## Async Collections

### BlockingCollection 

#### 📝 Articles

- [BlockingCollection Overview](https://docs.microsoft.com/en-us/dotnet/standard/collections/thread-safe/blockingcollection-overview) 
- [Event-driven .NET: Concurrent Producer/Consumer using BlockingCollection](https://makolyte.com/event-driven-dotnet-concurrent-producer-consumer-using-blockingcollection/)
- [An introduction to BlockingCollection](https://weblogs.asp.net/morteza/an-introduction-to-blockingcollection)



## Async Stream And IEnumerableAsync

### 📝 Articles

- [Use streaming in ASP.NET Core SignalR](https://docs.microsoft.com/en-us/aspnet/core/signalr/streaming?view=aspnetcore-5.0)
- [Async Streams](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/proposals/csharp-8.0/async-streams)
- [Iterating with Async Enumerables in C# 8](https://docs.microsoft.com/en-us/archive/msdn-magazine/2019/november/csharp-iterating-with-async-enumerables-in-csharp-8)
- [Async Streams with IAsyncEnumerable in .NET Core 3](https://anthonychu.ca/post/async-streams-dotnet-core-3-iasyncenumerable/)
- [IAsyncEnumerable Is Your Friend, Even In .NET Core 2.x](https://btburnett.com/csharp/2019/12/01/iasyncenumerable-is-your-friend.html)
- [Asynchronous streams in C# 8.0](https://blog.miguelbernard.com/asynchronous-streams)
- [gRPC and C# 8 Async stream](https://laurentkempe.com/2019/09/18/gRPC-and-csharp-8-Async-stream/)
- [gRPC and C# 8 Async stream cancellation](https://laurentkempe.com/2019/09/25/gRPC-and-csharp-8-Async-stream-cancellation/)

## Lazy Initialization

### 📝 Articles
- [Lazy Initialization](https://docs.microsoft.com/en-us/dotnet/framework/performance/lazy-initialization)

## Iterators

### 📝 Articles

- [Iterators](https://bettersolutions.com/csharp/collections/iterators.htm)

- [Iterators (C#)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/iterators)

- [yield (C# Reference)](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/yield)

- [Iterators, iterator blocks and data pipelines](https://csharpindepth.com/articles/StreamingAndIterators)

- [IEnumerator Interface](https://docs.microsoft.com/en-us/dotnet/api/system.collections.ienumerator?view=net-5.0)

- [IEnumerableT Interface](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.ienumerable-1?view=net-5.0)



## Channels

### 📹 Videos
- [C# Channels Explained (System.Threading.Channels)](https://www.youtube.com/watch?v=E0Ld7ZgE4oY)
- [Working with Channels in .NET](https://channel9.msdn.com/Shows/On-NET/Working-with-Channels-in-NET)


### 📝 Articles
- [An Introduction to System.Threading.Channels - Stephen Toub](https://devblogs.microsoft.com/dotnet/an-introduction-to-system-threading-channels/)
- [Using Channels In C# .NET Core – Part 1 – Getting Started](https://dotnetcoretutorials.com/2020/11/24/using-channels-in-net-core-part-1-getting-started/)
- [Using Channels In C# .NET Core – Part 2 – Advanced Channels](https://dotnetcoretutorials.com/2020/11/24/using-channels-in-net-core-part-2-advanced-channels/)
- [Using Channels In C# .NET Core – Part 3 – Understanding Back Pressure](https://dotnetcoretutorials.com/2020/11/24/using-channels-in-net-core-part-3-understanding-back-pressure/)
- [AN INTRODUCTION TO SYSTEM.THREADING.CHANNELS](https://www.stevejgordon.co.uk/an-introduction-to-system-threading-channels)
- [Producer/consumer pipelines with System.Threading.Channels](https://blog.maartenballiauw.be/post/2020/08/26/producer-consumer-pipelines-with-system-threading-channels.html)
- [C# Channels - Publish / Subscribe Workflows](https://deniskyashif.com/2019/12/08/csharp-channels-part-1/)
- [C# Channels - Timeout and Cancellation](https://deniskyashif.com/2019/12/11/csharp-channels-part-2/)
- [C# Channels - Async Data Pipelines](https://deniskyashif.com/2020/01/07/csharp-channels-part-3/)
- [How to implement Producer/Consumer with System.Threading.Channels](https://www.davideguida.com/how-to-implement-producer-consumer-with-system-threading-channels/)
- [How to implement Producer/Consumer with System.Threading.Channels](https://www.davideguida.com/consuming-message-queues-using-net-core-background-workers-part-4-adding-system-threading-channels/)
- [What's the Difference between Channel and ConcurrentQueue in C#?](https://jeremybytes.blogspot.com/2021/02/whats-difference-between-channel-and.html)

### 🔖 Samples

- [https://github.com/deniskyashif/trydotnet-channels](https://github.com/deniskyashif/trydotnet-channels)



## Libraries
- [Nito.AsyncEx](https://github.com/StephenCleary/AsyncEx)
  > A helper library for the Task-Based Asynchronous Pattern (TAP).

- [Microsoft.VisualStudio.Threading](https://github.com/microsoft/vs-threading)
  > Async synchronization primitives, async collections, TPL and dataflow extensions. The JoinableTaskFactory allows synchronously blocking the UI thread for async work. 

- [AsyncEnumerator](https://github.com/Dasync/AsyncEnumerable)
  > Introduces `IAsyncEnumerable`, `IAsyncEnumerator`, `ForEachAsync()`, and `ParallelForEachAsync()` and other useful stuff to use with async-await 

- [AsyncIO.DotNet](https://github.com/firenero/AsyncIO)
  > Easy-to-use library for common async IO file system operations. 

- [NeoSmart.AsyncLock](https://github.com/neosmart/AsyncLock)
  > A C# lock replacement for async/await, supporting recursion/re-entrance and asynchronous waits. 



## Code Analyzers

- [Microsoft.VisualStudio.Threading.Analyzers](https://b2n.ir/777981)
  > Static code analyzer to detect common mistakes or potential issues regarding threading and async coding. 

- [AsyncFixer](https://github.com/semihokur/AsyncFixer)
  > AsyncFixer helps developers in finding and correcting common async/await misuses (i.e., anti-patterns). 

- [ConfigureAwaitChecker.Analyzer](https://github.com/cincuranet/ConfigureAwaitChecker)
  > Checks for `ConfigureAwait(false)` usage. 

- [Lindhart.Analyser.MissingAwaitWarning](https://github.com/ykoksen/unused-task-warning)
  > Compiler analyser to generate Warnings whenever a Task is not awaited nor assigned to a variable.  

 
<div align="right">
  <b><a href="#contents">↥ Back To Top</a></b>
</div>

## Other Resources

- [Stephen Toub Blog](https://devblogs.microsoft.com/pfxteam/author/toub/)
- [Links about async/await in C#](https://www.meziantou.net/links-async-await-csharp.htm)
- [Marc Gravell Blog](https://blog.marcgravell.com/)

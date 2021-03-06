---
layout: page
title: Change log
---
{% include JB/setup %}

# 1.0.0-rc3
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-rc3)

October 2nd, 2015

This is an stabilization release, with several bug fixes. There is only one known bug, and the analyzer that is affected is disabled.
We will continue to focus on stabilization until 1.0.0 is ready.
Any new fixes will end up on the `master` branch.
New analyzers and fixers will continue to go on the `vnext` branch and will not be on our `1.0.0` release.

This release is still targetting the final version of Visual Studio 2015 (RTM, version `14.0.23107.0 D14REL`), as will the next ones. This release targets the `1.0.0` version of the Roslyn API (Microsoft.CodeAnalysis.*).
This release will not work on pre-release versions of VS 2015.

There are no new analyzers or code fixes in this release.

## Stats:

* 68 Analyzers in C#, 65 Code fixes, 3 Fix all
* 23 Analyzers in VB, 18 Code fixes
* 1682 tests
* 91% code coverage

## Known issues:

* &#35;468 CC0013 (user ternary) rule should be more careful with nullable types. (VB)
* &#35;493 CC0009 eats pragmas and trivia
* &#35;496 'TernaryOperatorWithAddignmentCodeFixProvider' encountered and error (CC0013 and CC0014)
* &#35;501 BUG on CC0008 and CC0009 (ObjectInitializer) when used with collection
* &#35;514 CC0017 Change to auto property fix all not working
* &#35;521 CC0013 Should check for a common type and cast is necessary

When the analyzer/code fix impacts the resulting code we disable it by default, you need to enable those that are disabled to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-rc3), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-rc3)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-rc3) and the detailed [changelog](https://github.com/code-cracker/code-cracker/blob/d303e7d534a29d940194a62d07235dd40574a1ca/CHANGELOG.md). For the commits, see the [full changelog](https://github.com/code-cracker/code-cracker/compare/v1.0.0-rc2...v1.0.0-rc3).

---

# 1.0.0-rc2
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-rc2)

August 19th, 2015

This release is still targetting the final version of Visual Studio 2015 (RTM, version `14.0.23107.0 D14REL`), as will the next ones. This release targets the `1.0.0` version of the Roslyn API (Microsoft.CodeAnalysis.*).
This release will not work on pre-release versions of VS 2015.

This is an stabilization release, with several bug fixes. There is only one known bug, and the analyzer that is affected is disabled.
We will continue to focus on stabilization until 1.0.0 is ready.
Any new fixes will end up on the `master` branch.
New analyzers and fixers will continue to go on the `vnext` branch and will not be on our `1.0.0` release.

## Stats:

* 68 Analyzers in C#, 65 Code fixes, 3 Fix all
* 23 Analyzers in VB, 18 Code fixes
* 1543 tests
* 91% code coverage

## Known issues:

* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)

When the analyzer/code fix impacts the resulting code we disable it by default, you need to enable those that are disabled to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-rc2), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-rc2)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-rc2).

---

# 1.0.0-rc1
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-rc1)

July 22nd, 2015

This release is the first one targeting the final version of Visual Studio 2015 (RTM, version `14.0.23107.0 D14REL`). This release targets the `1.0.0` version of the Roslyn API (Microsoft.CodeAnalysis.*).
The nuget package format has been updated from RC to RTM and this release will not work on pre-release versions of VS 2015.

From now on we will focus on stabilization and performance. There are only 3 known bugs, and we have some performance work to do. This work will end up on the `master` branch.
New analyzers and fixers will now go to a `vnext` branch and will not be on our `1.0.0` release.

## Stats:

* 68 Analyzers in C#, 65 Code fixes, 3 Fix all
* 23 Analyzers in VB, 18 Code fixes
* 1543 tests
* 91% code coverage

## Known issues:

* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)
* &#35;408 nameof(x) suggested before x is declared (CC0021)
* &#35;412 DocumentationCreateMissingParametersCodeFixProvider throws when there are only remarks (CC0090)

When the analyzer/code fix impacts the resulting code we disable it by default, you need to enable those that are disabled to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-rc1), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-rc1)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-rc1).

---

# 1.0.0-beta1
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-beta1)

July 3rd, 2015

This release is still targeting Visual Studio 2015 RC, as we wait for the RTM on July 20th.
The only bug present at the time is one that is due to a bug on Roslyn itself.
This is most likely our last pre-release as we prepare for the VS RTM. The next release will most likely be 1.0.0.

## Stats:

* 67 Analyzers in C#, 63 Code fixes, 3 Fix all
* 23 Analyzers in VB, 18 Code fixes
* 1529 tests
* 91% code coverage

## Known issues:

* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)

When the analyzer/code fix impacts the resulting code we disable it by default, you need to enable those that are disabled to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-beta1), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-beta1)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-beta1).

---

# 1.0.0-alpha6
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha6)

May 31st, 2015

This release is updated to target the 1.0.0-rc2 Roslyn Analyzers API, which works with Visual Studio 2015 RC.
We have also focuses heavily on fixing all our bugs. The only bugs left are one that is due to a bug on Roslyn itself and a recently discovered one.
We have been working hard on making CodeCracker more resilient. We started working on fix all tests, and have increased the code coverage, which was already high. It should continue to increase in the next releases. In this release we have surpassed the 1000 tests mark for the C# project alone!

## Stats:

* 64 Analyzers in C#, 57 Code fixes, 3 Fix all
* 22 Analyzers in VB, 17 Code fixes
* 1371 tests
* 91% code coverage

## Known issues:

* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)
* &#35;359 Nameof analyzer being raised on self referencing initialization statement (CC0021)

When the analyzer/code fix impacts the resulting code we disable it by default, you need to enable those that are disabled to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-alpha6), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-alpha6)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-alpha6).

---

# 1.0.0-alpha5
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha5)

Apr 25th, 2015

This release still targets the 1.0.0-rc1 Roslyn Analyzers API, which works with Visual Studio 2015 CTP 6.
We have updated CodeCracker in this release so it does not raise diagnostics on generated code. See issue 260 for more information on this subject. We have also focuses heavily on fixing all our bugs, only one remains, and it is due to a bug on Roslyn itself.

## Stats:

* 58 Analyzers in C#, 50 Code fixes
* 21 Analyzers in VB, 17 Code fixes
* 1186 tests
* 90% code coverage

## Known issues:

* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)

The above analyzer is disabled by default, you need to enable it to be able to use it.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-alpha5), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-alpha5)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-alpha5).

---

# 1.0.0-alpha4
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha4)

Mar 3rd, 2015

This release targets the 1.0.0-rc1 Roslyn Analyzers API, which works with Visual Studio 2015 CTP 6.
This release we also started taking better care of how code fix work when working on the "fix all" scenarios, when the whole document, project or solution is fixed.

## Stats:

* 53 Analyzers in C#, 48 Code fixes
* 20 Analyzers in VB, 17 Code fixes
* 936 tests
* 91% code coverage

## Known issues:

* &#35;95 Several small problems on DisposablesShouldCallSuppressFinalizeAnalyzer (CC0029)
* &#35;192 Null Reference on ConvertToExpressionBodiedMemberAnalyzer (CC0038)
* &#35;262 Incorrect diagnostic on CallExtensionMethodAsExtensionAnalyzer (CC0026)
* &#35;290 Incorrect diagnostic on RemovePrivateMethodNeverUsedAnalyzer (CC0068)
* &#35;291 Incorrect diagnostic on UnusedParametersAnalyzer (CC0057)
* &#35;293 Incorrect diagnostic on NoPrivateReadonlyFieldAnalyzer (CC0074)

All the above analyzers are disabled by default, you need to enable them to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-alpha4), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-alpha4)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

For a list of what worked on see the [corresponding milestone](https://github.com/code-cracker/code-cracker/issues?q=milestone%3A1.0.0-alpha4).

---

# 1.0.0-alpha3
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha3)

Jan 31st, 2015

This release targets the 1.0.0.0-beta2 Roslyn Analyzers API, which works with Visual Studio 2015 CTP 5.
This is our first release with Visual Basic.

## Stats:

* 52 Analyzers in C#
* 8 Analyzers in VB
* 724 tests
* 89% code coverage

## Known issues:

* &#35;192 Null Reference on ConvertToExpressionBodiedMemberAnalyzer
* &#35;95 Several small problems on DisposablesShouldCallSuppressFinalizeAnalyzer

All the above analyzers are disabled by default, you need to enable them to be able to use them.

As usual, you should go to Nuget ([C#](https://www.nuget.org/packages/codecracker.CSharp/1.0.0-alpha3), [VB](https://www.nuget.org/packages/codecracker.VisualBasic/1.0.0-alpha3)) to get the packages or download the extension on the Visual Studio Extensions Gallery ([C#](https://visualstudiogallery.msdn.microsoft.com/ab588981-91a5-478c-8e65-74d0ff450862), [VB](https://visualstudiogallery.msdn.microsoft.com/1a5f9551-e831-4812-abd0-ac48603fc2c1)).

---

# 1.0.0-alpha2
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha2)

Dec 15, 2014

---

# 1.0.0-alpha1
[Download](https://github.com/code-cracker/code-cracker/releases/tag/v1.0.0-alpha1)

Nov 12, 2014

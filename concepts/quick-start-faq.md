---
title: Microsoft Graph 快速入门 FAQ
description: 此 FAQ 解答了与 Microsoft Graph 快速入门相关的问题。
author: jasonjoh
ms.author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 00e1d3d20276c888f2f22d7e62f7434da282bca9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806821"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="a4781-103">Microsoft Graph 快速入门 FAQ</span><span class="sxs-lookup"><span data-stu-id="a4781-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="a4781-104">此 FAQ 解答了与 [Microsoft Graph 快速启动](https://developer.microsoft.com/graph/quick-start)相关的问题。</span><span class="sxs-lookup"><span data-stu-id="a4781-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="a4781-105">常规设计</span><span class="sxs-lookup"><span data-stu-id="a4781-105">General design</span></span>

<span data-ttu-id="a4781-106">快速启动示例展示了如何使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="a4781-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="a4781-107">在这些示例中，只需通过一次身份验证即可访问两项服务：Microsoft 帐户和 Outlook。</span><span class="sxs-lookup"><span data-stu-id="a4781-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="a4781-108">每个快速启动均均会访问 Microsoft 帐户用户个人资料中的信息，并显示其日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="a4781-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="a4781-109">快速启动分为四步：</span><span class="sxs-lookup"><span data-stu-id="a4781-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="a4781-110">选择平台</span><span class="sxs-lookup"><span data-stu-id="a4781-110">Select your platform</span></span>
- <span data-ttu-id="a4781-111">获取应用 ID（客户端 ID）</span><span class="sxs-lookup"><span data-stu-id="a4781-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="a4781-112">生成示例</span><span class="sxs-lookup"><span data-stu-id="a4781-112">Build the sample</span></span>
- <span data-ttu-id="a4781-113">登录，然后查看日历上的事件</span><span class="sxs-lookup"><span data-stu-id="a4781-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="a4781-114">完成快速启动后，即表示应用程序可供运行。</span><span class="sxs-lookup"><span data-stu-id="a4781-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="a4781-115">快速启动示例常见问题</span><span class="sxs-lookup"><span data-stu-id="a4781-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="a4781-116">此部分解答了快速启动示例的内容方面的问题。</span><span class="sxs-lookup"><span data-stu-id="a4781-116">This section answers questions about the contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="a4781-117">不通过快速启动页面下载可以获取快速启动代码吗？</span><span class="sxs-lookup"><span data-stu-id="a4781-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="a4781-118">当然可以！</span><span class="sxs-lookup"><span data-stu-id="a4781-118">Absolutely!</span></span> <span data-ttu-id="a4781-119">每个快速启动下载都是基于 [Microsoft Graph 教程](tutorials.yml)，因此，可以通过其他两种方法获取相同的源代码：</span><span class="sxs-lookup"><span data-stu-id="a4781-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.yml), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="a4781-120">按分步教程操作，自己构建代码。</span><span class="sxs-lookup"><span data-stu-id="a4781-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="a4781-121">从相应的 GitHub 存储库下载完整的项目，然后按照自述文件中的说明配置和运行示例。</span><span class="sxs-lookup"><span data-stu-id="a4781-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> [!NOTE]
> <span data-ttu-id="a4781-122">我们正在为当前已有快速启动示例的平台创建教程。</span><span class="sxs-lookup"><span data-stu-id="a4781-122">We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="a4781-123">因此，某些快速启动还没有相应的教程。</span><span class="sxs-lookup"><span data-stu-id="a4781-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="a4781-124">教程和 GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="a4781-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="a4781-125">下表列出了每个快速启动示例对应的教程和 GitHub 存储库。</span><span class="sxs-lookup"><span data-stu-id="a4781-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="a4781-126">快速启动</span><span class="sxs-lookup"><span data-stu-id="a4781-126">Quick start</span></span> | <span data-ttu-id="a4781-127">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-127">Tutorial</span></span> | <span data-ttu-id="a4781-128">GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="a4781-128">GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="a4781-129">Android</span><span class="sxs-lookup"><span data-stu-id="a4781-129">Android</span></span> | [<span data-ttu-id="a4781-130">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-130">Tutorial</span></span>](/graph/tutorials/android) | [<span data-ttu-id="a4781-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-131">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-android) |
| <span data-ttu-id="a4781-132">Angular</span><span class="sxs-lookup"><span data-stu-id="a4781-132">Angular</span></span> | [<span data-ttu-id="a4781-133">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="a4781-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-134">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="a4781-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="a4781-135">ASP.NET MVC</span></span> | [<span data-ttu-id="a4781-136">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-136">Tutorial</span></span>](/learn/modules/msgraph-build-aspnetmvc-apps) | [<span data-ttu-id="a4781-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-137">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="a4781-138">iOS Swift</span><span class="sxs-lookup"><span data-stu-id="a4781-138">iOS Swift</span></span> | <span data-ttu-id="a4781-139">手册(/graph/tutorials/ios-swift</span><span class="sxs-lookup"><span data-stu-id="a4781-139">[Tutorial](/graph/tutorials/ios-swift</span></span> | [<span data-ttu-id="a4781-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-140">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-ios-swift) |
| <span data-ttu-id="a4781-141">iOS Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4781-141">iOS Objective-C</span></span> | <span data-ttu-id="a4781-142">手册(/graph/tutorials/ios-objectivec</span><span class="sxs-lookup"><span data-stu-id="a4781-142">[Tutorial](/graph/tutorials/ios-objectivec</span></span> | [<span data-ttu-id="a4781-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-143">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-ios-objectivec) |
| <span data-ttu-id="a4781-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="a4781-144">Node.js</span></span> | [<span data-ttu-id="a4781-145">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="a4781-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-146">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="a4781-147">PHP</span><span class="sxs-lookup"><span data-stu-id="a4781-147">PHP</span></span> | [<span data-ttu-id="a4781-148">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="a4781-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-149">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="a4781-150">Python</span><span class="sxs-lookup"><span data-stu-id="a4781-150">Python</span></span> | [<span data-ttu-id="a4781-151">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="a4781-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-152">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="a4781-153">React</span><span class="sxs-lookup"><span data-stu-id="a4781-153">React</span></span> | [<span data-ttu-id="a4781-154">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-154">Tutorial</span></span>](/graph/tutorials/react) | [<span data-ttu-id="a4781-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-155">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-reactspa) |
| <span data-ttu-id="a4781-156">Ruby</span><span class="sxs-lookup"><span data-stu-id="a4781-156">Ruby</span></span> | [<span data-ttu-id="a4781-157">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-157">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="a4781-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-158">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="a4781-159">UWP</span><span class="sxs-lookup"><span data-stu-id="a4781-159">UWP</span></span> | [<span data-ttu-id="a4781-160">教程</span><span class="sxs-lookup"><span data-stu-id="a4781-160">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="a4781-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-161">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="a4781-162">Xamarin</span><span class="sxs-lookup"><span data-stu-id="a4781-162">Xamarin</span></span> | <span data-ttu-id="a4781-163">手册(/graph/tutorials/xamarin</span><span class="sxs-lookup"><span data-stu-id="a4781-163">[Tutorial](/graph/tutorials/xamarin</span></span> | [<span data-ttu-id="a4781-164">GitHub</span><span class="sxs-lookup"><span data-stu-id="a4781-164">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-xamarin) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="a4781-165">为什么所有快速启动示例都没有展示高级身份验证用例？</span><span class="sxs-lookup"><span data-stu-id="a4781-165">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="a4781-166">通过快速启动示例，大家认识了身份验证和 Microsoft Graph API 调用。</span><span class="sxs-lookup"><span data-stu-id="a4781-166">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="a4781-167">可以在 [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) 文档中了解与其他身份验证流相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="a4781-167">You can learn more about other authentication flows in the [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="a4781-168">使用快速启动时发生意外错误或遇到问题，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="a4781-168">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="a4781-169">如果无法正常使用快速启动，请在对应的 GitHub 存储库中报告问题。</span><span class="sxs-lookup"><span data-stu-id="a4781-169">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="known-issues"></a><span data-ttu-id="a4781-170">已知问题</span><span class="sxs-lookup"><span data-stu-id="a4781-170">Known issues</span></span>

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a><span data-ttu-id="a4781-171">ASP.NET 快速启动在运行时显示错误：找不到部分路径“[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe”。</span><span class="sxs-lookup"><span data-stu-id="a4781-171">ASP.NET quick start displays an error when running it: Cannot find a part of the path '[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe'.</span></span>

<span data-ttu-id="a4781-172">这是由 [Visual Studio 和 Roslyn 编译器的问题](https://github.com/dotnet/roslyn/issues/15556)引起的。</span><span class="sxs-lookup"><span data-stu-id="a4781-172">This is caused by an [issue with Visual Studio and the Roslyn compiler](https://github.com/dotnet/roslyn/issues/15556).</span></span> <span data-ttu-id="a4781-173">以下选项之一应该可解决该错误。</span><span class="sxs-lookup"><span data-stu-id="a4781-173">One of the following options should resolve the error.</span></span>

- <span data-ttu-id="a4781-174">在解决方案资源管理器中卸载/重新加载项目</span><span class="sxs-lookup"><span data-stu-id="a4781-174">Unload/reload project in Solution Explorer</span></span>
- <span data-ttu-id="a4781-175">清理/重新构建解决方案</span><span class="sxs-lookup"><span data-stu-id="a4781-175">Clean/Rebuild solution</span></span>
- <span data-ttu-id="a4781-176">升级 NuGet 包</span><span class="sxs-lookup"><span data-stu-id="a4781-176">Upgrade NuGet packages</span></span>

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a><span data-ttu-id="a4781-177">运行快速启动时，我遇到错误“AADSTS50011：请求中指定的回复 URL 与为应用程序配置的回复 URL 不匹配”。</span><span class="sxs-lookup"><span data-stu-id="a4781-177">I'm getting "AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application" when running a quick start.</span></span>

<span data-ttu-id="a4781-178">这表示快速启动的应用程序注册存在问题。</span><span class="sxs-lookup"><span data-stu-id="a4781-178">This indicates a problem with the application registration for the quick start.</span></span> <span data-ttu-id="a4781-179">从 [Microsoft Graph 快速入门页面](https://developer.microsoft.com/graph/quick-start)下载快速启动时，我们会为你创建应用程序注册，并配置与示例项目使用的默认 URL 匹配的回复 URL（也称为重定向 URL）。</span><span class="sxs-lookup"><span data-stu-id="a4781-179">When you download a quick start from the [Microsoft Graph Quick Starts page](https://developer.microsoft.com/graph/quick-start), we create the application registration for you, and configure a reply URL (also known as a redirect URL) that matches the default URL used by the sample project.</span></span> <span data-ttu-id="a4781-180">如果你更改了此 URL，则应用程序注册将不再匹配，并可能导致此错误。</span><span class="sxs-lookup"><span data-stu-id="a4781-180">If you change the URL, the app registration will no longer match and could cause this error.</span></span> <span data-ttu-id="a4781-181">若要解决此错误，请参阅快速启动项目附带的 README.md 文件，以获取有关如何创建应用程序注册并在示例代码中对其进行配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a4781-181">To resolve this error, consult the README.md file included with the quick start project for instructions on how to create an app registration and configure it in the sample code.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="a4781-182">找不到需要的内容？</span><span class="sxs-lookup"><span data-stu-id="a4781-182">Didn't find what you need?</span></span>

<span data-ttu-id="a4781-183">如果此 FAQ 无法解答在使用一个或多个快速启动时遇到的问题，请使用下面的“反馈”\*\*\*\* 部分告知我们。</span><span class="sxs-lookup"><span data-stu-id="a4781-183">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>

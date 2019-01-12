---
title: Microsoft Graph 快速入门 FAQ
description: 此 FAQ 解答了与 Microsoft Graph 快速入门相关的问题。
author: jasonjoh
ms.author: jasonjoh
ms.date: 12/13/2018
localization_priority: Normal
ms.openlocfilehash: 457b82813420b8771a5e59e9723f11885388c7b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834942"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="d02f2-103">Microsoft Graph 快速入门 FAQ</span><span class="sxs-lookup"><span data-stu-id="d02f2-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="d02f2-104">此 FAQ 解答了与 [Microsoft Graph 快速启动](https://developer.microsoft.com/graph/quick-start)相关的问题。</span><span class="sxs-lookup"><span data-stu-id="d02f2-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="d02f2-105">常规设计</span><span class="sxs-lookup"><span data-stu-id="d02f2-105">General design</span></span>

<span data-ttu-id="d02f2-106">快速启动示例展示了如何使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d02f2-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="d02f2-107">在这些示例中，只需通过一次身份验证即可访问两项服务：Microsoft 帐户和 Outlook。</span><span class="sxs-lookup"><span data-stu-id="d02f2-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="d02f2-108">每个快速启动均均会访问 Microsoft 帐户用户个人资料中的信息，并显示其日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="d02f2-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="d02f2-109">快速启动分为四步：</span><span class="sxs-lookup"><span data-stu-id="d02f2-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="d02f2-110">选择平台</span><span class="sxs-lookup"><span data-stu-id="d02f2-110">Select your platform</span></span>
- <span data-ttu-id="d02f2-111">获取应用 ID（客户端 ID）</span><span class="sxs-lookup"><span data-stu-id="d02f2-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="d02f2-112">生成示例</span><span class="sxs-lookup"><span data-stu-id="d02f2-112">Build the sample</span></span>
- <span data-ttu-id="d02f2-113">登录，然后查看日历上的事件</span><span class="sxs-lookup"><span data-stu-id="d02f2-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="d02f2-114">完成快速启动后，即表示应用程序可供运行。</span><span class="sxs-lookup"><span data-stu-id="d02f2-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="d02f2-115">快速启动示例常见问题</span><span class="sxs-lookup"><span data-stu-id="d02f2-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="d02f2-116">此部分解答了快速启动示例的内容方面的问题。</span><span class="sxs-lookup"><span data-stu-id="d02f2-116">This section answers questions about the contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="d02f2-117">不通过快速启动页面下载可以获取快速启动代码吗？</span><span class="sxs-lookup"><span data-stu-id="d02f2-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="d02f2-118">当然可以！</span><span class="sxs-lookup"><span data-stu-id="d02f2-118">Absolutely!</span></span> <span data-ttu-id="d02f2-119">每个快速启动下载都是基于 [Microsoft Graph 教程](tutorials.md)，因此，可以通过其他两种方法获取相同的源代码：</span><span class="sxs-lookup"><span data-stu-id="d02f2-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.md), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="d02f2-120">按分步教程操作，自己构建代码。</span><span class="sxs-lookup"><span data-stu-id="d02f2-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="d02f2-121">从相应的 GitHub 存储库下载完整的项目，然后按照自述文件中的说明配置和运行示例。</span><span class="sxs-lookup"><span data-stu-id="d02f2-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> <span data-ttu-id="d02f2-122">**注释：** 我们正在为当前已有快速启动示例的平台创建教程。</span><span class="sxs-lookup"><span data-stu-id="d02f2-122">**Note:** We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="d02f2-123">因此，某些快速启动还没有相应的教程。</span><span class="sxs-lookup"><span data-stu-id="d02f2-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="d02f2-124">教程和 GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="d02f2-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="d02f2-125">下表列出了每个快速启动示例对应的教程和 GitHub 存储库。</span><span class="sxs-lookup"><span data-stu-id="d02f2-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="d02f2-126">快速启动</span><span class="sxs-lookup"><span data-stu-id="d02f2-126">Quick start</span></span> | <span data-ttu-id="d02f2-127">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-127">Tutorial</span></span> | <span data-ttu-id="d02f2-128">GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="d02f2-128">GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="d02f2-129">Android</span><span class="sxs-lookup"><span data-stu-id="d02f2-129">Android</span></span> | <span data-ttu-id="d02f2-130">无</span><span class="sxs-lookup"><span data-stu-id="d02f2-130">None</span></span> | [<span data-ttu-id="d02f2-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-131">GitHub</span></span>](https://github.com/microsoftgraph/android-java-connect-sample) |
| <span data-ttu-id="d02f2-132">Angular</span><span class="sxs-lookup"><span data-stu-id="d02f2-132">Angular</span></span> | [<span data-ttu-id="d02f2-133">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="d02f2-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-134">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="d02f2-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="d02f2-135">ASP.NET MVC</span></span> | [<span data-ttu-id="d02f2-136">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-136">Tutorial</span></span>](/graph/tutorials/aspnet) | [<span data-ttu-id="d02f2-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-137">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="d02f2-138">iOS Swift</span><span class="sxs-lookup"><span data-stu-id="d02f2-138">iOS Swift</span></span> | <span data-ttu-id="d02f2-139">无</span><span class="sxs-lookup"><span data-stu-id="d02f2-139">None</span></span> | [<span data-ttu-id="d02f2-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-140">GitHub</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| <span data-ttu-id="d02f2-141">iOS Objective-C</span><span class="sxs-lookup"><span data-stu-id="d02f2-141">iOS Objective-C</span></span> | <span data-ttu-id="d02f2-142">无</span><span class="sxs-lookup"><span data-stu-id="d02f2-142">None</span></span> | [<span data-ttu-id="d02f2-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-143">GitHub</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| <span data-ttu-id="d02f2-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="d02f2-144">Node.js</span></span> | [<span data-ttu-id="d02f2-145">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="d02f2-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-146">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="d02f2-147">PHP</span><span class="sxs-lookup"><span data-stu-id="d02f2-147">PHP</span></span> | [<span data-ttu-id="d02f2-148">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="d02f2-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-149">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="d02f2-150">Python</span><span class="sxs-lookup"><span data-stu-id="d02f2-150">Python</span></span> | [<span data-ttu-id="d02f2-151">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="d02f2-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-152">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="d02f2-153">Ruby</span><span class="sxs-lookup"><span data-stu-id="d02f2-153">Ruby</span></span> | [<span data-ttu-id="d02f2-154">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-154">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="d02f2-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-155">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="d02f2-156">UWP</span><span class="sxs-lookup"><span data-stu-id="d02f2-156">UWP</span></span> | [<span data-ttu-id="d02f2-157">教程</span><span class="sxs-lookup"><span data-stu-id="d02f2-157">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="d02f2-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-158">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="d02f2-159">Xamarin</span><span class="sxs-lookup"><span data-stu-id="d02f2-159">Xamarin</span></span> | <span data-ttu-id="d02f2-160">无</span><span class="sxs-lookup"><span data-stu-id="d02f2-160">None</span></span> | [<span data-ttu-id="d02f2-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="d02f2-161">GitHub</span></span>](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="d02f2-162">为什么所有快速启动示例都没有展示高级身份验证用例？</span><span class="sxs-lookup"><span data-stu-id="d02f2-162">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="d02f2-163">通过快速启动示例，大家认识了身份验证和 Microsoft Graph API 调用。</span><span class="sxs-lookup"><span data-stu-id="d02f2-163">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="d02f2-164">可以在 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) 文档中了解与其他身份验证流相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="d02f2-164">You can learn more about other authentication flows in the [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="d02f2-165">使用快速启动时发生意外错误或遇到问题，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="d02f2-165">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="d02f2-166">如果无法正常使用快速启动，请在对应的 GitHub 存储库中报告问题。</span><span class="sxs-lookup"><span data-stu-id="d02f2-166">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="d02f2-167">找不到需要的内容？</span><span class="sxs-lookup"><span data-stu-id="d02f2-167">Didn't find what you need?</span></span>

<span data-ttu-id="d02f2-168">如果此 FAQ 无法解答在使用一个或多个快速启动时遇到的问题，请使用下面的“反馈”\*\*\*\* 部分告知我们。</span><span class="sxs-lookup"><span data-stu-id="d02f2-168">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>

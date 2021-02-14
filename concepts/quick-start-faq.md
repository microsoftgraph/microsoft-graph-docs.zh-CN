---
title: Microsoft Graph 快速入门 FAQ
description: 此 FAQ 解答了与 Microsoft Graph 快速入门相关的问题。
author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 71cd53990d76456d20bdcf21fcf7a92cbde16ff2
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239602"
---
# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph 快速入门 FAQ

此 FAQ 解答了与 [Microsoft Graph 快速启动](https://developer.microsoft.com/graph/quick-start)相关的问题。

## <a name="general-design"></a>常规设计

快速启动示例展示了如何使用 Microsoft Graph。 在这些示例中，只需通过一次身份验证即可访问两项服务：Microsoft 帐户和 Outlook。 每个快速启动均均会访问 Microsoft 帐户用户个人资料中的信息，并显示其日历中的事件。

快速启动分为四步：

- 选择平台
- 获取应用 ID（客户端 ID）
- 生成示例
- 登录，然后查看日历上的事件

完成快速启动后，即表示应用程序可供运行。

## <a name="prerequisites"></a>先决条件

所有快速入门示例都需要访问邮箱位于 Outlook.com 上的个人 Microsoft 帐户，或具有 Exchange Online 邮箱的 Microsoft 工作或学校帐户。 如果你没有 Microsoft 帐户，则有两种获取免费帐户的选项：

- 你可以 [注册新的个人 Microsoft 帐户](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1)。
- 你可以 [注册 Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program) ，获取免费的 Microsoft 365 订阅。

## <a name="general-quick-start-sample-questions"></a>快速启动示例常见问题

<!-- markdownlint-disable MD026 -->

此部分解答了快速启动示例的内容方面的问题。

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>不通过快速启动页面下载可以获取快速启动代码吗？

当然可以！ 每个快速启动下载都是基于 [Microsoft Graph 教程](tutorials.yml)，因此，可以通过其他两种方法获取相同的源代码：

- 按分步教程操作，自己构建代码。
- 从相应的 GitHub 存储库下载完整的项目，然后按照自述文件中的说明配置和运行示例。

#### <a name="tutorials-and-github-repositories"></a>教程和 GitHub 存储库

下表列出了每个快速启动示例对应的教程和 GitHub 存储库。

| 快速启动 | 教程 | GitHub 存储库 |
|-------------|----------|-------------------|
| Android | [教程](/graph/tutorials/android) | [GitHub](https://github.com/microsoftgraph/msgraph-training-android) |
| Angular | [教程](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [教程](/learn/modules/msgraph-build-aspnetmvc-apps) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | [教程](/graph/tutorials/ios-swift) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-swift) |
| iOS Objective-C | [教程](/graph/tutorials/ios-objectivec) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-objectivec) |
| Node.js | [教程](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [教程](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [教程](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| React | [教程](/graph/tutorials/react) | [GitHub](https://github.com/microsoftgraph/msgraph-training-reactspa) |
| Ruby | [教程](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [教程](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | [教程](/graph/tutorials/xamarin) | [GitHub](https://github.com/microsoftgraph/msgraph-training-xamarin) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>为什么所有快速启动示例都没有展示高级身份验证用例？

通过快速启动示例，大家认识了身份验证和 Microsoft Graph API 调用。 可以在 [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) 文档中了解与其他身份验证流相关的更多信息。

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>使用快速启动时发生意外错误或遇到问题，该怎么办？

如果无法正常使用快速启动，请在对应的 GitHub 存储库中报告问题。

## <a name="known-issues"></a>已知问题

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a>ASP.NET 快速启动在运行时显示错误：找不到部分路径“[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe”。

这是由 [Visual Studio 和 Roslyn 编译器的问题](https://github.com/dotnet/roslyn/issues/15556)引起的。 以下选项之一应该可解决该错误。

- 在解决方案资源管理器中卸载/重新加载项目
- 清理/重新构建解决方案
- 升级 NuGet 包

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a>运行快速启动时，我遇到错误“AADSTS50011：请求中指定的回复 URL 与为应用程序配置的回复 URL 不匹配”。

这表示快速启动的应用程序注册存在问题。 从 [Microsoft Graph 快速入门页面](https://developer.microsoft.com/graph/quick-start)下载快速启动时，我们会为你创建应用程序注册，并配置与示例项目使用的默认 URL 匹配的回复 URL（也称为重定向 URL）。 如果你更改了此 URL，则应用程序注册将不再匹配，并可能导致此错误。 若要解决此错误，请参阅快速启动项目附带的 README.md 文件，以获取有关如何创建应用程序注册并在示例代码中对其进行配置的说明。

### <a name="after-signing-in-im-told-i-need-admin-approval"></a>登录后，告诉我需要管理员批准。

登录其中一个快速入门示例后，你可能会看到一条消息，显示"需要管理员批准"XXX 教程需要访问组织中只有管理员可以授予的资源的权限。 请让管理员授予对此应用的权限，然后你才能使用它。" 这不是示例的 Bug！ 任何快速启动均不会请求任何默认情况下需要管理员 *同意的* Graph 权限范围。 租户管理员可以禁止你同意他们尚未批准的任何应用的 Graph 权限范围。 在这种情况下，你将看到此错误。

你需要与管理员合作以获得批准、使用个人 Microsoft 帐户 (Outlook.com) 或将测试 Microsoft 365 租户与 Exchange Online 一同使用。

## <a name="didnt-find-what-you-need"></a>找不到需要的内容？

如果此 FAQ 无法解答在使用一个或多个快速启动时遇到的问题，请使用下面的“反馈”部分告知我们。

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

## <a name="general-quick-start-sample-questions"></a>快速启动示例常见问题

<!-- markdownlint-disable MD026 -->

此部分解答了快速启动示例的内容方面的问题。

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>不通过快速启动页面下载可以获取快速启动代码吗？

当然可以！ 每个快速启动下载都是基于 [Microsoft Graph 教程](tutorials.md)，因此，可以通过其他两种方法获取相同的源代码：

- 按分步教程操作，自己构建代码。
- 从相应的 GitHub 存储库下载完整的项目，然后按照自述文件中的说明配置和运行示例。

> **注释：** 我们正在为当前已有快速启动示例的平台创建教程。 因此，某些快速启动还没有相应的教程。

#### <a name="tutorials-and-github-repositories"></a>教程和 GitHub 存储库

下表列出了每个快速启动示例对应的教程和 GitHub 存储库。

| 快速启动 | 教程 | GitHub 存储库 |
|-------------|----------|-------------------|
| Android | 无 | [GitHub](https://github.com/microsoftgraph/android-java-connect-sample) |
| Angular | [教程](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [教程](/graph/tutorials/aspnet) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | 无 | [GitHub](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| iOS Objective-C | 无 | [GitHub](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| Node.js | [教程](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [教程](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [教程](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| Ruby | [教程](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [教程](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | 无 | [GitHub](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>为什么所有快速启动示例都没有展示高级身份验证用例？

通过快速启动示例，大家认识了身份验证和 Microsoft Graph API 调用。 可以在 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) 文档中了解与其他身份验证流相关的更多信息。

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>使用快速启动时发生意外错误或遇到问题，该怎么办？

如果无法正常使用快速启动，请在对应的 GitHub 存储库中报告问题。

## <a name="didnt-find-what-you-need"></a>找不到需要的内容？

如果此 FAQ 无法解答在使用一个或多个快速启动时遇到的问题，请使用下面的“反馈”**** 部分告知我们。

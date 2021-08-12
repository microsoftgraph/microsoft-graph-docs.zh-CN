---
title: 云通信入门
description: 了解如何使用机器人响应客户的需求并促进协作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a977c2a81d40679eb3029bdfaf7560dd744fc9439e7a650e63d470198883ab0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246505"
---
# <a name="get-started-with-cloud-communications"></a>云通信入门

Microsoft 中的云通信 API Graph通过各种通信相关功能（如通话和联机会议）为应用和服务如何与用户交互添加了新的维度。 本文介绍如何使用机器人响应客户的需求并促进协作。

## <a name="prerequisites"></a>先决条件

在开始使用之前，熟悉以下内容会很有帮助：

- [Azure Active Directory (](/azure/active-directory/fundamentals/active-directory-whatis) Azure AD) 服务如何帮助员工登录和访问资源。
- [Azure Bot 服务](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0)及其功能。

## <a name="register-a-bot"></a>注册自动程序

术语"服务应用程序"和"bot"可以互换使用。 可以直接通过 Azure 门户创建自动程序 [，](https://azure.microsoft.com/features/azure-portal/) 也可以注册未托管在 Azure 上的自动程序。 有关机器人注册过程的更多详细信息，请参阅 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 

为了在以后简化操作，了解 Azure AD 中 [不同类型的权限非常有用](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) 。 具有委派权限的应用需要登录用户。 基于应用程序的权限不需要登录用户，通常可以作为后台服务运行。

注册自动程序后，如果你想要将机器人添加到[Microsoft Teams，请确保](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)你了解如何使用[app Studio](/microsoftteams/platform/get-started/get-started-app-studio)并定义所需的元数据。

## <a name="manage-the-state-of-the-bot"></a>管理自动程序的状态

注册自动程序后，决定是希望基于音频和视频的媒体是应用程序托管的还是 [服务托管的](cloud-communications-media.md)。 在高级别上，这涉及到决定是否要访问原始媒体实时流。

接下来，你可以决定是最适合自动程序是有 [状态还是无状态](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)。

### <a name="stateless-bots"></a>无状态机器人

任何虚拟机都可以处理任何自动程序实例，这意味着如果一台计算机关闭，另一台计算机可以处理它。 这使得解决方案具有弹性。

另一方面，共享缓存（如 REDIS）需要可供所有虚拟机访问。

### <a name="stateful-bots"></a>有状态自动程序

虚拟机一次只能处理一个自动程序实例。 由于所有状态都位于一台计算机中，因此没有任何额外的内存检查或 REDIS 缓存检查。

缺点是，由于自动程序实例仅位于一台计算机中，因此它无法复原。

>**注意：** 服务托管的媒体机器人可以是有状态或无状态的。 应用程序托管的媒体机器人必须具有状态，才能使用[Bot Media SDK。](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)

## <a name="use-the-sdks"></a>使用 SDK

以下 SDK 可用于C#。 我们将在未来提供对其他语言的支持。

- 如果你使用的是无状态 **机器人**，请安装 [Graph通信核心 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core)。
- 如果你使用的是有状态 **机器人**，请安装 Graph [Communications Calling SDK。](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)

## <a name="examples"></a>示例

了解如何使用有状态机器人实现不同的方案，例如使用应用程序托管的媒体[](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls)或服务托管的媒体应答传入呼叫。

有关更多示例，请参阅 [通信示例存储库](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)。

## <a name="privacy-and-compliance"></a>隐私与合规性

在 API 请求中，不应以任何客户端生成的 ID (（如标头或请求正文中的方案 ID、请求 ID 或其他相关 ID) ）发送敏感数据。 这些 ID 将记录在服务器端进行诊断。

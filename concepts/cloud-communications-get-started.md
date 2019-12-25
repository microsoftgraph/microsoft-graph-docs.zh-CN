---
title: 云通信入门
description: 了解如何使用 bot 来响应客户需求并促进协作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ae04e60079a789125dd6a818c19ec625eaac1443
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871577"
---
# <a name="get-started-with-cloud-communications"></a>云通信入门

Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。 本文介绍如何使用 bot 来响应客户需求并促进协作。

## <a name="prerequisites"></a>先决条件

Beore 开始时，熟悉以下内容会很有帮助：

- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) （azure AD）以及服务如何帮助员工登录和访问资源。
- [Azure Bot 服务](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0)及其功能。

## <a name="register-a-bot"></a>注册 bot

术语 "服务应用程序" 和 "bot" 可互换使用。 您可以通过[azure 门户](https://azure.microsoft.com/features/azure-portal/)直接创建机器人，也可以注册不在 azure 上托管的 bot。 有关 bot 注册过程的更多详细信息，请参阅[注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 

为更轻松地执行更多操作，了解 Azure AD 中的不同[类型的权限](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions)非常有用。 具有委派权限的应用程序需要已登录用户。 基于应用程序的权限不需要登录用户，并且通常可以作为后台服务运行。

注册你的 bot 后，如果你想要[将你的 bot 添加到 Microsoft 团队](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)，请确保了解如何使用[应用程序 studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio)并定义所需的元数据。

## <a name="manage-the-state-of-the-bot"></a>管理机器人的状态

注册你的 bot 后，决定是希望基于音频和视频的媒体是[应用程序托管的还是托管服务的](cloud-communications-media.md)。 从较高的层次来看，这需要决定是否要访问原始媒体的实时流。

接下来，你可以决定是否最适合你的 bot 进行[状态或无状态](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)。

### <a name="stateless-bots"></a>无状态 bot

任何虚拟机都可以处理任何 bot 实例，这意味着如果一台计算机出现故障，另一台可能会处理它。 这将生成弹性解决方案。

另一方面，共享缓存（如 REDIS）需要对所有虚拟机都是可访问的。

### <a name="stateful-bots"></a>有状态的 bot

虚拟机一次只能处理一个 bot 实例。 由于所有状态都在一台计算机上，因此没有任何额外的内存检查或 REDIS 缓存检查。

缺点是，由于 bot 实例只在一台计算机上，因此不能恢复。

>**注意：** 服务托管的媒体 bot 可以是有状态的，也可以是无状态的。 应用程序托管的媒体 bot 必须处于状态，才能使用[Bot 媒体 SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)。

## <a name="use-the-sdks"></a>使用 Sdk

C # 中提供了以下 Sdk。 我们将在将来为其他语言提供支持。

- 如果您使用的是**无状态**bot，请安装[GRAPH 通信核心 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core)。
- 如果您使用的是有**状态**的 bot，请安装[GRAPH 通信呼叫 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)。

## <a name="examples"></a>示例

了解如何使用有状态的 bot 实施不同的方案，例如，使用应用程序托管或服务承载的媒体[应答传入呼叫](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls)。

有关更多示例，请参阅[通信示例存储库](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)。

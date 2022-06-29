---
title: 云通信 API 入门
description: 使用 Microsoft Graph 中的云通信 API 为客户生成机器人。 了解如何注册机器人，然后管理机器人的状态。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: e2b380108d06abc987fdf92564a1ecf17289d9c5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442153"
---
# <a name="get-started-with-the-cloud-communications-api"></a>云通信 API 入门

可以使用 Microsoft Graph 中的云通信 API 生成机器人来响应客户的需求并促进协作。 本文介绍如何注册机器人，然后管理机器人的状态。

## <a name="prerequisites"></a>先决条件

在开始之前，熟悉以下内容会很有帮助：

- [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) 以及服务如何帮助员工登录和访问资源。
- [Azure 机器人服务](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0&preserve-view=true)及其功能。

## <a name="register-a-bot"></a>注册机器人

可以互换使用术语“服务应用程序”和“机器人”。 可以直接通过[Azure 门户](https://azure.microsoft.com/features/azure-portal/)创建机器人，也可以注册未托管在 Azure 上的机器人。 有关机器人注册过程的更多详细信息，请参阅 [注册调用机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 

为了在以后简化操作，了解 Azure AD [中不同类型的权限](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) 很有帮助。 具有委派权限的应用需要登录用户。 基于应用程序的权限不需要登录用户，并且通常可以作为后台服务运行。

注册机器人后，如果要将 [机器人添加到 Microsoft Teams](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)，请确保了解如何使用 [应用工作室](/microsoftteams/platform/get-started/get-started-app-studio) 并定义所需的元数据。

## <a name="manage-the-state-of-the-bot"></a>管理机器人的状态

注册机器人后，确定是要将基于音频和视频的媒体 [托管还是服务托管](cloud-communications-media.md)。 在高级别上，这涉及到决定是否要访问原始媒体的实时流。

接下来，你可以决定机器人最好是 [有状态还是无状态](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)。

### <a name="stateless-bots"></a>无状态机器人

任何虚拟机都可以处理任何机器人实例，这意味着如果一台计算机发生关闭，另一台计算机可以处理它。 这可以实现复原解决方案。

另一方面，共享缓存（如 REDIS）需要可供所有虚拟机访问。

### <a name="stateful-bots"></a>有状态机器人

虚拟机一次只能处理一个机器人实例。 由于所有状态都在一台计算机上，因此没有任何额外的内存检查或 REDIS 缓存检查。

缺点是，由于机器人实例仅在一台计算机上，因此没有那么可复原。

> [!NOTE]
> 服务托管的媒体机器人可以是有状态的或无状态的。 应用程序托管的媒体机器人必须是有状态的，才能使用 [Bot Media SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)。

## <a name="use-the-sdks"></a>使用 SDK

以下 SDK 在 C# 中可用。 将来我们将为其他语言提供支持。

- 如果使用的是 **无状态** 机器人，请安装 [Graph Communications Core SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core)。
- 如果使用的是 **有状态** 机器人，请安装 [Graph Communications 呼叫 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)。

## <a name="examples"></a>示例

了解如何使用有状态机器人实现不同的方案，例如使用应用程序托管媒体或服务托管媒体 [接听传入呼叫](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) 。

有关更多示例，请参阅 [Communications 示例存储库](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)。

## <a name="privacy-and-compliance"></a>隐私与合规性

在对 API 的请求中，不应在任何客户端生成的 ID 中发送敏感数据， (例如方案 ID、请求 ID 或标头或请求正文中) 的其他相关 ID。 这些 ID 将记录在服务器端进行诊断。

## <a name="see-also"></a>另请参阅

- [云通信 API 概述](cloud-communications-concept-overview.md)
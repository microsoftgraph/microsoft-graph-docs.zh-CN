---
title: 使用 Microsoft Graph 的通知 REST API
description: 可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。
ms.localizationpriority: high
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 90233d1efd45d49475572a55e13b2555d597f5d5
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58694624"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>使用 Microsoft Graph 的通知 REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需向目标用户发布通知，平台即可向注册到该用户的所有设备终结点发送通知。 高级流如下所示：

1. 用户登录到你的应用程序，从而创建包含 Microsoft Graph 通知服务的订阅。 将向调用应用程序返回特定用户通知订阅 ID 或 UNSID。
2. 应用程序将此 UNSID 发送到应用程序服务。
3. 准备好发送通知时，应用程序服务[通过 Microsoft 标识平台进行身份验证](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow)，并通过 Microsoft Graph 通知服务发布通知，提供验证码、目标用户的 UNSID 以及通知负载。
4. Microsoft Graph 通知服务将通知扇出至具有活动订阅的用户的所有终结点。

此类以用户为中心的通知通过 [](../resources/projectrome-notification.md) 资源标识，存储在 Microsoft Graph 通知服务中。 随后可由客户端应用程序通过[客户端 SDK API](https://aka.ms/GNSDK) 访问和管理。 若不熟悉 Microsoft Graph 通知服务，请查看[通知概述](/graph/notifications-concept-overview)部分了解详细信息。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤
- 请参阅[通知资源](../resources/projectrome-notification.md)并创建通知，以与用户交互。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
- 按照[集成概述](/graph/notifications-integration-e2e-overview)主题中的步骤开始客户端集成。
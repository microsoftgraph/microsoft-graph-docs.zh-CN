---
title: 通过应用程序服务创建和发送通知（已弃用）
description: 可以使用 Microsoft Graph API 为用户创建和发送通知（已弃用）。
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 302375137bb2408bcd6be5ad737cf34cc7d6ee70
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447133"
---
# <a name="create-and-send-a-notification-from-your-app-service-deprecated"></a>通过应用程序服务创建和发送通知（已弃用）

> [!IMPORTANT]
> Microsoft Graph 通知 API 已弃用，并且已于 2022 年 1 月停止返回数据。 有关其他通知体验，请参阅 [Microsoft Azure 通知中心](/azure/notification-hubs)。 更多相关信息，请参阅博客文章 [停用 Microsoft Graph 通知 API (beta 版本)](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/)。

可以使用 Microsoft Graph API 为用户创建和发送通知。 通知存储在 Microsoft Graph 通知服务中，并发送到目标用户登录的所有设备上的所有应用客户端。 

若要向你的用户发送通知，你的应用程序服务将：
1. 向 Microsoft 标识平台[进行身份验证](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow)。
2. 使用身份验证令牌将通知发布到 Microsoft Graph API，并以[用户通知订阅 ID](/graph/api/notifications-post)（创建订阅时从应用客户端获取）定位用户。

> [!NOTE]
> 为获得简化的身份验证故事，建议使用客户端上新的和改进的轻型[通知 SDK](https://aka.ms/GNSDK) 以及用户通知订阅 ID 来接收通知和管理通知状态。 或者，你可以通过委派权限代表用户发布通知，你的应用服务将需要维护访问令牌和刷新令牌，但不建议这样做。 若要详细了解 OAuth 2.0 OBO 流，请参阅[代表流中使用委派用户标识的服务到服务调用](/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)。 


## <a name="guaranteed-delivery-on-ios"></a>iOS 上的保证传递

在如 iOS 的平台上，在特定电源条件下，原始数据通知可能由于批处理而延迟传递，或者根本无法到达目标终结点。 为了向 iOS 上的用户传递高优先级通知，Microsoft Graph 通知平台允许你指定原始到可视 toast 通知“回退”选项，该选项会自动向目标 iOS 设备发送可视 toast 通知，从而确保你的用户近实时获得通知。 若要了解如何利用回退选项，请参阅[通知资源](/graph/api/resources/projectrome-notification.md)。  

## <a name="getting-started"></a>入门
若要了解你的应用服务如何开始向你的用户发送通知，请参阅[通知](/graph/api/resources/projectrome-notification)和我们的[应用服务示例](https://aka.ms/gnsample-appservice)。

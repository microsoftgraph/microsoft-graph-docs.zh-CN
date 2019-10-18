---
title: 通过应用程序服务创建和发送通知
description: '将应用程序服务设置为通过 Microsoft Graph 向不同客户端发送以用户为中心的通知。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: cf40087aff3956a88f79197482db8126bbe8d96c
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683508"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a>通过应用程序服务创建和发送通知

可以使用 Microsoft Graph API 为用户创建和发送通知。 通知存储在活动源存储中，并发送到目标用户登录的所有设备上的所有应用客户端。 

## <a name="authentication"></a>身份验证

Microsoft Graph 通知要求你的应用程序服务使用代表 (OBO) 流向用户发布通知。 以下是身份验证流：

1.  用户使用其 Microsoft 或工作或学校帐户登录至你的应用程序。 登录时，标识服务将为你提供一个访问令牌。

2.  你将此访问令牌发送至应用程序服务。

3.  应用程序服务对标识服务进行身份验证，并且需要 OBO 令牌才能发送 Microsoft Graph 通知。

4.  标识服务返回基于 OBO 的令牌和刷新令牌。 应用程序服务可以使用此访问令牌向用户发布通知。

若要详细了解 OAuth 2.0 OBO 流，请参阅[代表流中使用委派用户标识的服务到服务调用](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)。 有关此流与 Microsoft Graph 通知如何搭配使用的详细信息，请参阅[应用程序服务示例](https://aka.ms/gnsample-appservice)。

> [!NOTE]
> Microsoft Graph 通知目前使用带有未来计划的 OBO 身份验证流，以此进一步简化此身份验证，并消除维护访问令牌和刷新令牌的需要。

有关 API 权限以及请求和响应标题的更多详细信息，请参阅 API 参考部分的[创建和发送通知](/graph/api/notifications-post)。 

---
title: 通过应用程序服务创建和发送通知
description: '将应用程序服务设置为通过 Microsoft Graph 向不同客户端发送以用户为中心的通知。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 1148c554b90fca5aeb56627e47a1d060f53f772e
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063251"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a>通过应用程序服务创建和发送通知

可以使用 Microsoft Graph API 为用户创建和发送通知。 通知存储于活动源存储区中，并且被发送至目标用户登录的所有设备的所有应用程序客户端上。请参阅以下内容，以了解如何进行身份验证、所需的权限范围、请求标题/正文和预期响应。

## <a name="authentication"></a>身份验证

Microsoft Graph 通知要求你的应用程序服务使用代表 (OBO) 流向用户发布通知。 以下是身份验证流：

1.  用户使用其 Microsoft 或工作或学校帐户登录至你的应用程序。 登录时，标识服务将为你提供一个访问令牌。

2.  你将此访问令牌发送至应用程序服务。

3.  应用程序服务对标识服务进行身份验证，并且需要 OBO 令牌才能发送 Microsoft Graph 通知。

4.  标识服务返回基于 OBO 的令牌和刷新令牌。 应用程序服务可以使用此访问令牌向用户发布通知。

若要详细了解 OAuth 2.0 OBO 流，请参阅[代表流中使用委派用户标识的服务到服务调用](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)。 有关此流与 Microsoft Graph 通知如何搭配使用的详细信息，请参阅[应用程序服务示例](https://aka.ms/gnsample-appservice)。

> [!NOTE]
> Microsoft Graph 通知目前使用带有未来计划的 OBO 身份验证流，以此进一步简化此身份验证，并消除维护访问令牌和刷新令牌的需要。

有关 API 权限以及请求和响应标题的更多详细信息，请参阅 API 参考部分的[创建和发送通知](/graph/api/notifications-post)。 

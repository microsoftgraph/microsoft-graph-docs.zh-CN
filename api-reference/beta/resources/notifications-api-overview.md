---
title: 使用 Microsoft Graph 的通知 REST API
description: 你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。 将通过委派权限和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 5c6d2dd846a03430f5bae65ef3b4a6838ccf7841
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036479"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>使用 Microsoft Graph 的通知 REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。 将通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。
此类以用户为中心的通知通过[通知](../resources/projectrome-notification.md)资源标识，存储在 Microsoft Graph 中。 随后可由发布应用程序通过[客户端 SDK API](https://github.com/Microsoft/project-rome) 访问和管理。 

## <a name="next-steps"></a>后续步骤
- 请参阅[通知资源](../resources/projectrome-notification.md)并创建通知，以与用户交互。 
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
- 按照[集成概述](/graph/notification-integration-e2e-overview)中列出的步骤开始客户端集成。

---
title: 在 Microsoft Graph 中使用 REST API 的通知
description: 在 Microsoft Graph 中的通知 API 可用于向用户发送推送通知。 只需目标的用户帐户以发送通知，以及在平台将传递到所有设备终结点的通知。 通知 API 请求执行代表通过委派的权限和[通知的权限]( /graph/permissions_reference)，用户可用于或者是 Microsoft 帐户或工作或学校帐户。
localization_priority: Priority
ms.openlocfilehash: 04787cb9a9b589036020651934041b4fc399adb1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853023"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>在 Microsoft Graph 中使用 REST API 的通知

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Microsoft Graph 中的通知 API 可用于向用户发送推送通知。 只需目标的用户帐户以发送通知，以及在平台将传递到所有设备终结点的通知。 通知 API 请求执行代表通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[通知的权限]( /graph/permissions_reference)，用户可用于或者是 Microsoft 帐户或工作或学校帐户。
以用户为中心的通知的此类型由[通知](../resources/projectrome-notification.md)资源，存储在 Microsoft Graph。 它可以然后访问和管理发布应用程序通过[项目 Rome SDK Api](https://github.com/Microsoft/project-rome)。 

## <a name="next-steps"></a>后续步骤
- 请参阅[通知资源](../resources/projectrome-notification.md)和创建通知来与您的用户。 
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。

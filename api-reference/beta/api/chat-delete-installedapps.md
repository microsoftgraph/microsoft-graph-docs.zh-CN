---
title: 在聊天中卸载应用
description: 卸载（删除）聊天中安装的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a463fd0c57f707c766367b2bd6e7abc326d35aa2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607500"
---
# <a name="uninstall-app-in-a-chat"></a>在聊天中卸载应用

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

卸载在[聊天](../resources/chat.md)中安装的[应用](../resources/teamsapp.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All |

## <a name="http-request"></a>HTTP 请求

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a>响应

如果成功，此方法将返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面的示例将从指定的聊天中卸载应用。
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat delete installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

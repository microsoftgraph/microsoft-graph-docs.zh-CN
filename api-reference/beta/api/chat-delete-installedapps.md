---
title: 在聊天中卸载应用
description: 卸载（删除）聊天中安装的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 954567f3d899f432922edb2c1c618814282043c4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658581"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="7c76a-103">在聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="7c76a-103">Uninstall app in a chat</span></span>

<span data-ttu-id="7c76a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c76a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c76a-105">卸载在[聊天](../resources/chat.md)中安装的[应用](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7c76a-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="7c76a-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，然后 **teamsApp** 将迅速从会议中删除。</span><span class="sxs-lookup"><span data-stu-id="7c76a-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c76a-107">权限</span><span class="sxs-lookup"><span data-stu-id="7c76a-107">Permissions</span></span>

<span data-ttu-id="7c76a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c76a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c76a-110">Permission type</span></span>      | <span data-ttu-id="7c76a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c76a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c76a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c76a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c76a-113">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="7c76a-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="7c76a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c76a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c76a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c76a-115">Not supported.</span></span>   |
|<span data-ttu-id="7c76a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c76a-116">Application</span></span> | <span data-ttu-id="7c76a-117">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="7c76a-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c76a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c76a-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="7c76a-119">响应</span><span class="sxs-lookup"><span data-stu-id="7c76a-119">Response</span></span>

<span data-ttu-id="7c76a-120">如果成功，此方法将返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7c76a-120">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c76a-121">示例</span><span class="sxs-lookup"><span data-stu-id="7c76a-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c76a-122">请求</span><span class="sxs-lookup"><span data-stu-id="7c76a-122">Request</span></span>

<span data-ttu-id="7c76a-123">下面的示例将从指定的聊天中卸载应用。</span><span class="sxs-lookup"><span data-stu-id="7c76a-123">The following example uninstalls an app from the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a><span data-ttu-id="7c76a-124">响应</span><span class="sxs-lookup"><span data-stu-id="7c76a-124">Response</span></span>

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

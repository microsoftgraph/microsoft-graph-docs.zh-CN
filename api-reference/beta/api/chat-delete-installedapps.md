---
title: 在聊天中卸载应用
description: 卸载（删除）聊天中安装的应用。
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3566191d894c2e98ccdb3d91c513f1581e6d6716
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971375"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="a8a6a-103">在聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="a8a6a-103">Uninstall app in a chat</span></span>

<span data-ttu-id="a8a6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a6a-105">卸载在[聊天](../resources/chat.md)中安装的[应用](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="a8a6a-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，然后 **teamsApp** 将迅速从会议中删除。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8a6a-107">权限</span><span class="sxs-lookup"><span data-stu-id="a8a6a-107">Permissions</span></span>

<span data-ttu-id="a8a6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8a6a-110">Permission type</span></span>      | <span data-ttu-id="a8a6a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8a6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8a6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a6a-113">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="a8a6a-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="a8a6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8a6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-115">Not supported.</span></span>   |
|<span data-ttu-id="a8a6a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8a6a-116">Application</span></span> | <span data-ttu-id="a8a6a-117">Chat.Manage.Chat\*、TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="a8a6a-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="a8a6a-118">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="a8a6a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8a6a-119">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="a8a6a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8a6a-120">Request headers</span></span>
|<span data-ttu-id="a8a6a-121">名称</span><span class="sxs-lookup"><span data-stu-id="a8a6a-121">Name</span></span>|<span data-ttu-id="a8a6a-122">说明</span><span class="sxs-lookup"><span data-stu-id="a8a6a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8a6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8a6a-123">Authorization</span></span>|<span data-ttu-id="a8a6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a6a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8a6a-126">Request body</span></span>
<span data-ttu-id="a8a6a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8a6a-128">响应</span><span class="sxs-lookup"><span data-stu-id="a8a6a-128">Response</span></span>

<span data-ttu-id="a8a6a-129">如果成功，此方法将返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-129">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8a6a-130">示例</span><span class="sxs-lookup"><span data-stu-id="a8a6a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8a6a-131">请求</span><span class="sxs-lookup"><span data-stu-id="a8a6a-131">Request</span></span>

<span data-ttu-id="a8a6a-132">下面的示例将从指定的聊天中卸载应用。</span><span class="sxs-lookup"><span data-stu-id="a8a6a-132">The following example uninstalls an app from the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8a6a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a6a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="a8a6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="a8a6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8a6a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8a6a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8a6a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8a6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8a6a-137">Java</span><span class="sxs-lookup"><span data-stu-id="a8a6a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8a6a-138">响应</span><span class="sxs-lookup"><span data-stu-id="a8a6a-138">Response</span></span>

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

---
title: 在聊天中卸载应用
description: 卸载（删除）聊天中安装的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3a2557a7fd4fc731ad0e528a16d54784e2915c7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958448"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="1e6ca-103">在聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="1e6ca-103">Uninstall app in a chat</span></span>

<span data-ttu-id="1e6ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e6ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e6ca-105">卸载在[聊天](../resources/chat.md)中安装的[应用](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="1e6ca-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，然后 **teamsApp** 将迅速从会议中删除。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e6ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="1e6ca-107">Permissions</span></span>

<span data-ttu-id="1e6ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e6ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e6ca-110">Permission type</span></span>      | <span data-ttu-id="1e6ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e6ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e6ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e6ca-113">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="1e6ca-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="1e6ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e6ca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-115">Not supported.</span></span>   |
|<span data-ttu-id="1e6ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e6ca-116">Application</span></span> | <span data-ttu-id="1e6ca-117">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="1e6ca-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e6ca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e6ca-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="1e6ca-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e6ca-119">Request headers</span></span>
|<span data-ttu-id="1e6ca-120">名称</span><span class="sxs-lookup"><span data-stu-id="1e6ca-120">Name</span></span>|<span data-ttu-id="1e6ca-121">说明</span><span class="sxs-lookup"><span data-stu-id="1e6ca-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e6ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e6ca-122">Authorization</span></span>|<span data-ttu-id="1e6ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e6ca-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e6ca-125">Request body</span></span>
<span data-ttu-id="1e6ca-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e6ca-127">响应</span><span class="sxs-lookup"><span data-stu-id="1e6ca-127">Response</span></span>

<span data-ttu-id="1e6ca-128">如果成功，此方法将返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-128">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1e6ca-129">示例</span><span class="sxs-lookup"><span data-stu-id="1e6ca-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e6ca-130">请求</span><span class="sxs-lookup"><span data-stu-id="1e6ca-130">Request</span></span>

<span data-ttu-id="1e6ca-131">下面的示例将从指定的聊天中卸载应用。</span><span class="sxs-lookup"><span data-stu-id="1e6ca-131">The following example uninstalls an app from the specified chat.</span></span>


# <a name="http"></a>[<span data-ttu-id="1e6ca-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e6ca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="1e6ca-133">C#</span><span class="sxs-lookup"><span data-stu-id="1e6ca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e6ca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e6ca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e6ca-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e6ca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e6ca-136">Java</span><span class="sxs-lookup"><span data-stu-id="1e6ca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1e6ca-137">响应</span><span class="sxs-lookup"><span data-stu-id="1e6ca-137">Response</span></span>

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

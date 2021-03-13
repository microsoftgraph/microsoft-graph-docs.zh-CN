---
title: 获取聊天中安装的应用
description: 获取聊天中安装的应用。
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a83c9cf192d5c30ccdc8c3a88d5ac5c699e6d971
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775855"
---
# <a name="get-installed-app-in-chat"></a><span data-ttu-id="05d55-103">获取聊天中安装的应用</span><span class="sxs-lookup"><span data-stu-id="05d55-103">Get installed app in chat</span></span>

<span data-ttu-id="05d55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05d55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05d55-105">获取[聊天](../resources/chat.md)中安装的[应用](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="05d55-105">Get an [app](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05d55-106">权限</span><span class="sxs-lookup"><span data-stu-id="05d55-106">Permissions</span></span>

<span data-ttu-id="05d55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05d55-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05d55-109">Permission type</span></span>      | <span data-ttu-id="05d55-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05d55-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05d55-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05d55-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05d55-112">TeamsAppInstallation.ReadForChat、TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="05d55-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="05d55-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05d55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05d55-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05d55-114">Not supported.</span></span>    |
|<span data-ttu-id="05d55-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05d55-115">Application</span></span> | <span data-ttu-id="05d55-116">TeamsAppInstallation.ReadForChat.All、TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="05d55-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span>

## <a name="http-request"></a><span data-ttu-id="05d55-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05d55-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="05d55-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="05d55-118">Request headers</span></span>

|<span data-ttu-id="05d55-119">名称</span><span class="sxs-lookup"><span data-stu-id="05d55-119">Name</span></span>|<span data-ttu-id="05d55-120">说明</span><span class="sxs-lookup"><span data-stu-id="05d55-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05d55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05d55-121">Authorization</span></span>|<span data-ttu-id="05d55-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05d55-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="05d55-124">响应</span><span class="sxs-lookup"><span data-stu-id="05d55-124">Response</span></span>

<span data-ttu-id="05d55-125">如果成功，此方法将在响应正文中返回 `200 OK` 和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05d55-125">If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="05d55-126">示例</span><span class="sxs-lookup"><span data-stu-id="05d55-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="05d55-127">请求</span><span class="sxs-lookup"><span data-stu-id="05d55-127">Request</span></span>

<span data-ttu-id="05d55-128">下面的示例将获取在指定聊天中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="05d55-128">The following example gets an app installed in the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="05d55-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="05d55-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installedApps_in_chat"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="05d55-130">C#</span><span class="sxs-lookup"><span data-stu-id="05d55-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05d55-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05d55-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05d55-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05d55-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05d55-133">Java</span><span class="sxs-lookup"><span data-stu-id="05d55-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05d55-134">响应</span><span class="sxs-lookup"><span data-stu-id="05d55-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps/$entity",
    "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat get installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

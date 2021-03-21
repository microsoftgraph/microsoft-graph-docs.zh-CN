---
title: 将应用添加到聊天
description: 将应用安装到聊天。
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 682a43113d46509b8db5ae18ce01f749cc2836f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958235"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="7c210-103">将应用添加到聊天</span><span class="sxs-lookup"><span data-stu-id="7c210-103">Add app to chat</span></span>

<span data-ttu-id="7c210-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c210-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="7c210-105">将 [teamsApp](../resources/teamsapp.md) 安装到指定的[聊天](../resources/chat.md)中。</span><span class="sxs-lookup"><span data-stu-id="7c210-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="7c210-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，然后 **teamsApp** 将迅速安装到会议。</span><span class="sxs-lookup"><span data-stu-id="7c210-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get installed to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c210-107">权限</span><span class="sxs-lookup"><span data-stu-id="7c210-107">Permissions</span></span>

<span data-ttu-id="7c210-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c210-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c210-110">Permission type</span></span>      | <span data-ttu-id="7c210-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c210-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c210-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c210-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c210-113">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="7c210-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="7c210-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c210-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c210-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c210-115">Not supported.</span></span>    |
|<span data-ttu-id="7c210-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c210-116">Application</span></span> | <span data-ttu-id="7c210-117">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="7c210-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c210-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c210-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="7c210-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c210-119">Request headers</span></span>

| <span data-ttu-id="7c210-120">标头</span><span class="sxs-lookup"><span data-stu-id="7c210-120">Header</span></span>       | <span data-ttu-id="7c210-121">值</span><span class="sxs-lookup"><span data-stu-id="7c210-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c210-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c210-122">Authorization</span></span>  | <span data-ttu-id="7c210-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c210-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c210-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c210-125">Content-Type</span></span>  | <span data-ttu-id="7c210-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7c210-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c210-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c210-128">Request body</span></span>

<span data-ttu-id="7c210-129">请求正文应包含目录应用的生成应用 ID。</span><span class="sxs-lookup"><span data-stu-id="7c210-129">The request body should contain the catalog app's generated app ID.</span></span> <span data-ttu-id="7c210-130">有关详细信息，请参阅 [teamsApp 属性](../resources/teamsapp.md#properties)。</span><span class="sxs-lookup"><span data-stu-id="7c210-130">For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="7c210-131">响应</span><span class="sxs-lookup"><span data-stu-id="7c210-131">Response</span></span>

<span data-ttu-id="7c210-132">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7c210-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7c210-133">示例</span><span class="sxs-lookup"><span data-stu-id="7c210-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c210-134">请求</span><span class="sxs-lookup"><span data-stu-id="7c210-134">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="7c210-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c210-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
"teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="7c210-136">C#</span><span class="sxs-lookup"><span data-stu-id="7c210-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c210-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c210-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c210-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c210-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c210-139">Java</span><span class="sxs-lookup"><span data-stu-id="7c210-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7c210-140">响应</span><span class="sxs-lookup"><span data-stu-id="7c210-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat add installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

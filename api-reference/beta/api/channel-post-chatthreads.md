---
title: 创建聊天线程
description: 通过提供根邮件，在指定的通道中创建新的聊天线程。
ms.openlocfilehash: 9a2a35a086c6689d1b76a56b70cd3637ec23c3a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041684"
---
# <a name="create-chat-thread"></a><span data-ttu-id="1ab23-103">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="1ab23-103">Create chat thread</span></span>

> <span data-ttu-id="1ab23-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1ab23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ab23-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1ab23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ab23-106">通过提供根邮件，在指定的[频道](../resources/channel.md)中创建一个新的聊天线程。</span><span class="sxs-lookup"><span data-stu-id="1ab23-106">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ab23-107">权限</span><span class="sxs-lookup"><span data-stu-id="1ab23-107">Permissions</span></span>
<span data-ttu-id="1ab23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ab23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ab23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ab23-110">Permission type</span></span>      | <span data-ttu-id="1ab23-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ab23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ab23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ab23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ab23-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab23-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ab23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ab23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ab23-115">Not supported.</span></span>    |
|<span data-ttu-id="1ab23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ab23-116">Application</span></span> | <span data-ttu-id="1ab23-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ab23-117">Not supported.</span></span> |

> <span data-ttu-id="1ab23-118">目前，仅[委派权限](/graph/permissions-reference)支持此操作。</span><span class="sxs-lookup"><span data-stu-id="1ab23-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="1ab23-119">将来版本将支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="1ab23-119">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="1ab23-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ab23-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="1ab23-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ab23-121">Request headers</span></span>
| <span data-ttu-id="1ab23-122">名称</span><span class="sxs-lookup"><span data-stu-id="1ab23-122">Name</span></span>       | <span data-ttu-id="1ab23-123">类型</span><span class="sxs-lookup"><span data-stu-id="1ab23-123">Type</span></span> | <span data-ttu-id="1ab23-124">说明</span><span class="sxs-lookup"><span data-stu-id="1ab23-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ab23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ab23-125">Authorization</span></span>  | <span data-ttu-id="1ab23-126">string</span><span class="sxs-lookup"><span data-stu-id="1ab23-126">string</span></span>  | <span data-ttu-id="1ab23-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ab23-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ab23-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ab23-129">Request body</span></span>
<span data-ttu-id="1ab23-130">在请求正文中，提供[chatThread](../resources/chatthread.md)对象，其中包含 rootMessage 属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ab23-130">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="1ab23-131">响应</span><span class="sxs-lookup"><span data-stu-id="1ab23-131">Response</span></span>

<span data-ttu-id="1ab23-132">如果成功，此方法返回`201 Created`空响应正文的响应代码。</span><span class="sxs-lookup"><span data-stu-id="1ab23-132">If successful, this method returns `201 Created` response code with an empty reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="1ab23-133">示例</span><span class="sxs-lookup"><span data-stu-id="1ab23-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ab23-134">请求</span><span class="sxs-lookup"><span data-stu-id="1ab23-134">Request</span></span>
<span data-ttu-id="1ab23-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ab23-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="1ab23-136">目前，必须将 contentType 指定为一个整数，而不是字符串:"text"或"html"1 的 0。</span><span class="sxs-lookup"><span data-stu-id="1ab23-136">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="1ab23-137">将来 API 版本会修复此错误。</span><span class="sxs-lookup"><span data-stu-id="1ab23-137">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="1ab23-138">响应</span><span class="sxs-lookup"><span data-stu-id="1ab23-138">Response</span></span>

<span data-ttu-id="1ab23-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1ab23-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

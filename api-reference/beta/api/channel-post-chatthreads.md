---
title: 创建聊天线程
description: 通过提供根消息在指定频道中新建聊天线程。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ef8d341310296c810c433a23f0d29be166ca47c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511245"
---
# <a name="create-chat-thread"></a><span data-ttu-id="9e6dc-103">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="9e6dc-103">Create chat thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6dc-104">通过提供根消息在指定[频道](../resources/channel.md)中新建聊天线程。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-104">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e6dc-105">权限</span><span class="sxs-lookup"><span data-stu-id="9e6dc-105">Permissions</span></span>
<span data-ttu-id="9e6dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6dc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e6dc-108">Permission type</span></span>      | <span data-ttu-id="9e6dc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e6dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e6dc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e6dc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6dc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e6dc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e6dc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-113">Not supported.</span></span>    |
|<span data-ttu-id="9e6dc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e6dc-114">Application</span></span> | <span data-ttu-id="9e6dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-115">Not supported.</span></span> |

> <span data-ttu-id="9e6dc-116">目前，此操作只支持[委派权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-116">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="9e6dc-117">未来版本将支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-117">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="9e6dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e6dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="9e6dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e6dc-119">Request headers</span></span>
| <span data-ttu-id="9e6dc-120">名称</span><span class="sxs-lookup"><span data-stu-id="9e6dc-120">Name</span></span>       | <span data-ttu-id="9e6dc-121">类型</span><span class="sxs-lookup"><span data-stu-id="9e6dc-121">Type</span></span> | <span data-ttu-id="9e6dc-122">说明</span><span class="sxs-lookup"><span data-stu-id="9e6dc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e6dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e6dc-123">Authorization</span></span>  | <span data-ttu-id="9e6dc-124">string</span><span class="sxs-lookup"><span data-stu-id="9e6dc-124">string</span></span>  | <span data-ttu-id="9e6dc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e6dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e6dc-127">Request body</span></span>
<span data-ttu-id="9e6dc-128">在请求正文中，提供包含 rootMessage 属性的 [chatThread](../resources/chatthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-128">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="9e6dc-129">响应</span><span class="sxs-lookup"><span data-stu-id="9e6dc-129">Response</span></span>

<span data-ttu-id="9e6dc-130">如果成功，此方法将返回 `201 Created` 响应代码及空响应正文。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-130">If successful, this method returns a `201 Created` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e6dc-131">示例</span><span class="sxs-lookup"><span data-stu-id="9e6dc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e6dc-132">请求</span><span class="sxs-lookup"><span data-stu-id="9e6dc-132">Request</span></span>
<span data-ttu-id="9e6dc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-133">Here is an example of the request.</span></span>
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

> <span data-ttu-id="9e6dc-134">目前，contentType 必须指定为整数，而不是字符串：0 表示“文本”或 1 表示“html”。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-134">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="9e6dc-135">今后发布的 API 版本将修复此功能。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-135">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="9e6dc-136">响应</span><span class="sxs-lookup"><span data-stu-id="9e6dc-136">Response</span></span>

<span data-ttu-id="9e6dc-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9e6dc-137">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatthreads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

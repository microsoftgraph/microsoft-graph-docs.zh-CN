---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
ms.openlocfilehash: 33e38e321ff948f55213646cb9349db85176e989
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046026"
---
# <a name="get-conversation"></a><span data-ttu-id="94bfa-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="94bfa-103">Get conversation</span></span>

> <span data-ttu-id="94bfa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94bfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94bfa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94bfa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94bfa-106">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94bfa-106">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94bfa-107">权限</span><span class="sxs-lookup"><span data-stu-id="94bfa-107">Permissions</span></span>
<span data-ttu-id="94bfa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94bfa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94bfa-110">Permission type</span></span>      | <span data-ttu-id="94bfa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94bfa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94bfa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94bfa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94bfa-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="94bfa-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="94bfa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94bfa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94bfa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94bfa-115">Not supported.</span></span>    |
|<span data-ttu-id="94bfa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94bfa-116">Application</span></span> | <span data-ttu-id="94bfa-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="94bfa-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94bfa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94bfa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="94bfa-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94bfa-119">Optional query parameters</span></span>
<span data-ttu-id="94bfa-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="94bfa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94bfa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="94bfa-121">Request headers</span></span>
| <span data-ttu-id="94bfa-122">标头</span><span class="sxs-lookup"><span data-stu-id="94bfa-122">Header</span></span>       | <span data-ttu-id="94bfa-123">值</span><span class="sxs-lookup"><span data-stu-id="94bfa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94bfa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94bfa-124">Authorization</span></span>  | <span data-ttu-id="94bfa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94bfa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94bfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94bfa-127">Request body</span></span>
<span data-ttu-id="94bfa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94bfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94bfa-129">响应</span><span class="sxs-lookup"><span data-stu-id="94bfa-129">Response</span></span>

<span data-ttu-id="94bfa-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94bfa-130">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94bfa-131">示例</span><span class="sxs-lookup"><span data-stu-id="94bfa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94bfa-132">请求</span><span class="sxs-lookup"><span data-stu-id="94bfa-132">Request</span></span>
<span data-ttu-id="94bfa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94bfa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="94bfa-134">响应</span><span class="sxs-lookup"><span data-stu-id="94bfa-134">Response</span></span>
<span data-ttu-id="94bfa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94bfa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

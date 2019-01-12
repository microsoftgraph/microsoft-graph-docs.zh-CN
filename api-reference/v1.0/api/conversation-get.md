---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 174d5a5b5309348de5ebf01d38445d032d9e31ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980389"
---
# <a name="get-conversation"></a><span data-ttu-id="4ab15-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="4ab15-103">Get conversation</span></span>

<span data-ttu-id="4ab15-104">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ab15-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ab15-105">权限</span><span class="sxs-lookup"><span data-stu-id="4ab15-105">Permissions</span></span>
<span data-ttu-id="4ab15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ab15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab15-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ab15-108">Permission type</span></span>      | <span data-ttu-id="4ab15-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ab15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab15-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab15-111">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ab15-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="4ab15-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab15-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ab15-113">Not supported.</span></span>    |
|<span data-ttu-id="4ab15-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ab15-114">Application</span></span> | <span data-ttu-id="4ab15-115">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ab15-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab15-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ab15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ab15-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ab15-117">Optional query parameters</span></span>
<span data-ttu-id="4ab15-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ab15-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ab15-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ab15-119">Request headers</span></span>
| <span data-ttu-id="4ab15-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ab15-120">Header</span></span>       | <span data-ttu-id="4ab15-121">值</span><span class="sxs-lookup"><span data-stu-id="4ab15-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ab15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab15-122">Authorization</span></span>  | <span data-ttu-id="4ab15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ab15-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ab15-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ab15-125">Request body</span></span>
<span data-ttu-id="4ab15-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ab15-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab15-127">响应</span><span class="sxs-lookup"><span data-stu-id="4ab15-127">Response</span></span>

<span data-ttu-id="4ab15-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ab15-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ab15-129">示例</span><span class="sxs-lookup"><span data-stu-id="4ab15-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab15-130">请求</span><span class="sxs-lookup"><span data-stu-id="4ab15-130">Request</span></span>
<span data-ttu-id="4ab15-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ab15-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="4ab15-132">响应</span><span class="sxs-lookup"><span data-stu-id="4ab15-132">Response</span></span>
<span data-ttu-id="4ab15-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ab15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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

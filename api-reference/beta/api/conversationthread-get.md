---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以指定父对话和线程，或， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f53afdd5416e2973c79ce3ec47e5101d3126d20f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510510"
---
# <a name="get-conversationthread"></a><span data-ttu-id="227b8-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="227b8-104">Get conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="227b8-p102">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="227b8-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="227b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="227b8-107">Permissions</span></span>
<span data-ttu-id="227b8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="227b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="227b8-110">Permission type</span></span>      | <span data-ttu-id="227b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="227b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="227b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="227b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="227b8-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="227b8-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="227b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="227b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="227b8-115">Not supported.</span></span>    |
|<span data-ttu-id="227b8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="227b8-116">Application</span></span> | <span data-ttu-id="227b8-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="227b8-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="227b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="227b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="227b8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="227b8-119">Optional query parameters</span></span>
<span data-ttu-id="227b8-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="227b8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="227b8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="227b8-121">Request headers</span></span>
| <span data-ttu-id="227b8-122">标头</span><span class="sxs-lookup"><span data-stu-id="227b8-122">Header</span></span>       | <span data-ttu-id="227b8-123">值</span><span class="sxs-lookup"><span data-stu-id="227b8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="227b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="227b8-124">Authorization</span></span>  | <span data-ttu-id="227b8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="227b8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="227b8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="227b8-127">Request body</span></span>
<span data-ttu-id="227b8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="227b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="227b8-129">响应</span><span class="sxs-lookup"><span data-stu-id="227b8-129">Response</span></span>

<span data-ttu-id="227b8-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="227b8-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="227b8-131">示例</span><span class="sxs-lookup"><span data-stu-id="227b8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="227b8-132">请求</span><span class="sxs-lookup"><span data-stu-id="227b8-132">Request</span></span>
<span data-ttu-id="227b8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="227b8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="227b8-134">响应</span><span class="sxs-lookup"><span data-stu-id="227b8-134">Response</span></span>
<span data-ttu-id="227b8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="227b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

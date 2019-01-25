---
title: 列出线程
description: 获取组对话中的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: bdef7c4a5fe6d28772cff5ed0f286065595e1088
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519400"
---
# <a name="list-threads"></a><span data-ttu-id="86525-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="86525-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86525-104">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="86525-104">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="86525-105">注意：还可以 [获取组的所有线程](group-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="86525-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="86525-106">权限</span><span class="sxs-lookup"><span data-stu-id="86525-106">Permissions</span></span>
<span data-ttu-id="86525-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86525-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86525-109">Permission type</span></span>      | <span data-ttu-id="86525-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86525-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86525-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86525-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86525-112">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="86525-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="86525-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86525-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86525-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86525-114">Not supported.</span></span>    |
|<span data-ttu-id="86525-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86525-115">Application</span></span> | <span data-ttu-id="86525-116">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="86525-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86525-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86525-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86525-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86525-118">Optional query parameters</span></span>
<span data-ttu-id="86525-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86525-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="86525-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86525-120">Request headers</span></span>
| <span data-ttu-id="86525-121">标头</span><span class="sxs-lookup"><span data-stu-id="86525-121">Header</span></span>       | <span data-ttu-id="86525-122">值</span><span class="sxs-lookup"><span data-stu-id="86525-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86525-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86525-123">Authorization</span></span>  | <span data-ttu-id="86525-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86525-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86525-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86525-126">Request body</span></span>
<span data-ttu-id="86525-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86525-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86525-128">响应</span><span class="sxs-lookup"><span data-stu-id="86525-128">Response</span></span>

<span data-ttu-id="86525-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="86525-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86525-130">示例</span><span class="sxs-lookup"><span data-stu-id="86525-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86525-131">请求</span><span class="sxs-lookup"><span data-stu-id="86525-131">Request</span></span>
<span data-ttu-id="86525-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86525-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="86525-133">响应</span><span class="sxs-lookup"><span data-stu-id="86525-133">Response</span></span>
<span data-ttu-id="86525-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86525-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversation-list-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

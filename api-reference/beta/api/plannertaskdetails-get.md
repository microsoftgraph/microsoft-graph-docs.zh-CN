---
title: 获取 plannerTaskDetails
description: 检索 **plannertaskdetails** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 2c680470681e5b6e5640eb75e05e8ce7431fdc96
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413067"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="e809d-103">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="e809d-103">Get plannerTaskDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e809d-104">检索 **plannertaskdetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e809d-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e809d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e809d-105">Permissions</span></span>
<span data-ttu-id="e809d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e809d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e809d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e809d-108">Permission type</span></span>      | <span data-ttu-id="e809d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e809d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e809d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e809d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e809d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e809d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e809d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e809d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e809d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e809d-113">Not supported.</span></span>    |
|<span data-ttu-id="e809d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e809d-114">Application</span></span> | <span data-ttu-id="e809d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e809d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e809d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e809d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="e809d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e809d-117">Request headers</span></span>
| <span data-ttu-id="e809d-118">名称</span><span class="sxs-lookup"><span data-stu-id="e809d-118">Name</span></span>      |<span data-ttu-id="e809d-119">说明</span><span class="sxs-lookup"><span data-stu-id="e809d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e809d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e809d-120">Authorization</span></span>  | <span data-ttu-id="e809d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e809d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e809d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e809d-123">Request body</span></span>
<span data-ttu-id="e809d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e809d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e809d-125">响应</span><span class="sxs-lookup"><span data-stu-id="e809d-125">Response</span></span>

<span data-ttu-id="e809d-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerTaskDetails](../resources/plannertaskdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e809d-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="e809d-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="e809d-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e809d-130">示例</span><span class="sxs-lookup"><span data-stu-id="e809d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e809d-131">请求</span><span class="sxs-lookup"><span data-stu-id="e809d-131">Request</span></span>
<span data-ttu-id="e809d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e809d-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e809d-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e809d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e809d-134">C#</span><span class="sxs-lookup"><span data-stu-id="e809d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e809d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e809d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e809d-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="e809d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertaskdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e809d-137">响应</span><span class="sxs-lookup"><span data-stu-id="e809d-137">Response</span></span>
<span data-ttu-id="e809d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e809d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

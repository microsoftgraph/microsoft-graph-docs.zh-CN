---
title: 获取 plannerTaskDetails
description: 检索 **plannertaskdetails** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5168a3ead931869adaed189c0c52ef941df758e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264314"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="78e23-103">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="78e23-103">Get plannerTaskDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78e23-104">检索 **plannertaskdetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78e23-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="78e23-105">权限</span><span class="sxs-lookup"><span data-stu-id="78e23-105">Permissions</span></span>
<span data-ttu-id="78e23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e23-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e23-108">Permission type</span></span>      | <span data-ttu-id="78e23-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78e23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78e23-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78e23-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e23-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="78e23-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78e23-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e23-113">Not supported.</span></span>    |
|<span data-ttu-id="78e23-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e23-114">Application</span></span> | <span data-ttu-id="78e23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78e23-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="78e23-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e23-117">Request headers</span></span>
| <span data-ttu-id="78e23-118">名称</span><span class="sxs-lookup"><span data-stu-id="78e23-118">Name</span></span>      |<span data-ttu-id="78e23-119">说明</span><span class="sxs-lookup"><span data-stu-id="78e23-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78e23-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e23-120">Authorization</span></span>  | <span data-ttu-id="78e23-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78e23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78e23-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e23-123">Request body</span></span>
<span data-ttu-id="78e23-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78e23-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78e23-125">响应</span><span class="sxs-lookup"><span data-stu-id="78e23-125">Response</span></span>

<span data-ttu-id="78e23-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerTaskDetails](../resources/plannertaskdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78e23-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="78e23-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="78e23-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="78e23-130">示例</span><span class="sxs-lookup"><span data-stu-id="78e23-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78e23-131">请求</span><span class="sxs-lookup"><span data-stu-id="78e23-131">Request</span></span>
<span data-ttu-id="78e23-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e23-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
##### <a name="response"></a><span data-ttu-id="78e23-133">响应</span><span class="sxs-lookup"><span data-stu-id="78e23-133">Response</span></span>
<span data-ttu-id="78e23-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78e23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="78e23-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="78e23-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="78e23-138">C#</span><span class="sxs-lookup"><span data-stu-id="78e23-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78e23-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="78e23-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="78e23-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="78e23-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

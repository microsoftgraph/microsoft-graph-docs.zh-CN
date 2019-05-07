---
title: 列出计划
description: 检索 **plannerplan** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: c783a09ba7cef3dc2cf5a7d329d183ff2dae1e4e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611470"
---
# <a name="list-plans"></a><span data-ttu-id="93e35-103">列出计划</span><span class="sxs-lookup"><span data-stu-id="93e35-103">List plans</span></span>

<span data-ttu-id="93e35-104">检索 **plannerplan** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="93e35-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="93e35-105">权限</span><span class="sxs-lookup"><span data-stu-id="93e35-105">Permissions</span></span>
<span data-ttu-id="93e35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93e35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="93e35-108">Permission type</span></span>      | <span data-ttu-id="93e35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93e35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93e35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93e35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93e35-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e35-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93e35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93e35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e35-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="93e35-113">Not supported.</span></span>    |
|<span data-ttu-id="93e35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="93e35-114">Application</span></span> | <span data-ttu-id="93e35-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93e35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93e35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93e35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93e35-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="93e35-117">Optional query parameters</span></span>
<span data-ttu-id="93e35-118">此方法要求指定所有者[筛选器](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="93e35-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93e35-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93e35-119">Request headers</span></span>
| <span data-ttu-id="93e35-120">名称</span><span class="sxs-lookup"><span data-stu-id="93e35-120">Name</span></span>      |<span data-ttu-id="93e35-121">说明</span><span class="sxs-lookup"><span data-stu-id="93e35-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93e35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93e35-122">Authorization</span></span>  | <span data-ttu-id="93e35-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93e35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93e35-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="93e35-125">Request body</span></span>
<span data-ttu-id="93e35-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93e35-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93e35-127">响应</span><span class="sxs-lookup"><span data-stu-id="93e35-127">Response</span></span>

<span data-ttu-id="93e35-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="93e35-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="93e35-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="93e35-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="93e35-132">示例</span><span class="sxs-lookup"><span data-stu-id="93e35-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93e35-133">请求</span><span class="sxs-lookup"><span data-stu-id="93e35-133">Request</span></span>
<span data-ttu-id="93e35-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93e35-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
##### <a name="response"></a><span data-ttu-id="93e35-135">响应</span><span class="sxs-lookup"><span data-stu-id="93e35-135">Response</span></span>
<span data-ttu-id="93e35-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93e35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="93e35-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="93e35-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93e35-140">语言</span><span class="sxs-lookup"><span data-stu-id="93e35-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93e35-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="93e35-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plans-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

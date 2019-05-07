---
title: 获取 plannerBucket
description: 检索 **plannerBucket** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d30483be99ddcdac67334a6f62692b7322f8556d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33609398"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="d1fc4-103">获取 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d1fc4-103">Get plannerBucket</span></span>

<span data-ttu-id="d1fc4-104">检索 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-104">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1fc4-105">权限</span><span class="sxs-lookup"><span data-stu-id="d1fc4-105">Permissions</span></span>
<span data-ttu-id="d1fc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1fc4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1fc4-108">Permission type</span></span>      | <span data-ttu-id="d1fc4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1fc4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1fc4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1fc4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d1fc4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1fc4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1fc4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1fc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1fc4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-113">Not supported.</span></span>    |
|<span data-ttu-id="d1fc4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1fc4-114">Application</span></span> | <span data-ttu-id="d1fc4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1fc4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1fc4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1fc4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1fc4-117">Request headers</span></span>
| <span data-ttu-id="d1fc4-118">名称</span><span class="sxs-lookup"><span data-stu-id="d1fc4-118">Name</span></span>      |<span data-ttu-id="d1fc4-119">说明</span><span class="sxs-lookup"><span data-stu-id="d1fc4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1fc4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1fc4-120">Authorization</span></span>  | <span data-ttu-id="d1fc4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1fc4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1fc4-123">Request body</span></span>
<span data-ttu-id="d1fc4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1fc4-125">响应</span><span class="sxs-lookup"><span data-stu-id="d1fc4-125">Response</span></span>

<span data-ttu-id="d1fc4-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-126">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="d1fc4-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d1fc4-130">示例</span><span class="sxs-lookup"><span data-stu-id="d1fc4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1fc4-131">请求</span><span class="sxs-lookup"><span data-stu-id="d1fc4-131">Request</span></span>
<span data-ttu-id="d1fc4-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
##### <a name="response"></a><span data-ttu-id="d1fc4-133">响应</span><span class="sxs-lookup"><span data-stu-id="d1fc4-133">Response</span></span>
<span data-ttu-id="d1fc4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1fc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1fc4-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d1fc4-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1fc4-138">语言</span><span class="sxs-lookup"><span data-stu-id="d1fc4-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannerbucket-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1fc4-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1fc4-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannerbucket-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerbucket-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerbucket-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

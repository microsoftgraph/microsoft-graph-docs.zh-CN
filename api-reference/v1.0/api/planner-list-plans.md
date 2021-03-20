---
title: 列出计划
description: 检索 **plannerplan** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 4cf4fdbf93cea301e1ddd893d61a0f80664534c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941512"
---
# <a name="list-plans"></a><span data-ttu-id="33fc3-103">列出计划</span><span class="sxs-lookup"><span data-stu-id="33fc3-103">List plans</span></span>

<span data-ttu-id="33fc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33fc3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33fc3-105">检索 **plannerplan** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="33fc3-105">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="33fc3-106">权限</span><span class="sxs-lookup"><span data-stu-id="33fc3-106">Permissions</span></span>
<span data-ttu-id="33fc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33fc3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="33fc3-109">Permission type</span></span>      | <span data-ttu-id="33fc3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33fc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33fc3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33fc3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33fc3-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33fc3-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="33fc3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33fc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33fc3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fc3-114">Not supported.</span></span>    |
|<span data-ttu-id="33fc3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="33fc3-115">Application</span></span> | <span data-ttu-id="33fc3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fc3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33fc3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33fc3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33fc3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="33fc3-118">Optional query parameters</span></span>
<span data-ttu-id="33fc3-119">此方法要求指定所有者[筛选器](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="33fc3-119">This method requires owner [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33fc3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="33fc3-120">Request headers</span></span>
| <span data-ttu-id="33fc3-121">名称</span><span class="sxs-lookup"><span data-stu-id="33fc3-121">Name</span></span>      |<span data-ttu-id="33fc3-122">说明</span><span class="sxs-lookup"><span data-stu-id="33fc3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33fc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33fc3-123">Authorization</span></span>  | <span data-ttu-id="33fc3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33fc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33fc3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="33fc3-126">Request body</span></span>
<span data-ttu-id="33fc3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33fc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33fc3-128">响应</span><span class="sxs-lookup"><span data-stu-id="33fc3-128">Response</span></span>

<span data-ttu-id="33fc3-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33fc3-129">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="33fc3-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="33fc3-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="33fc3-133">示例</span><span class="sxs-lookup"><span data-stu-id="33fc3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33fc3-134">请求</span><span class="sxs-lookup"><span data-stu-id="33fc3-134">Request</span></span>
<span data-ttu-id="33fc3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33fc3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33fc3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="33fc3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="33fc3-137">C#</span><span class="sxs-lookup"><span data-stu-id="33fc3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33fc3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33fc3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33fc3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33fc3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33fc3-140">Java</span><span class="sxs-lookup"><span data-stu-id="33fc3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33fc3-141">响应</span><span class="sxs-lookup"><span data-stu-id="33fc3-141">Response</span></span>
<span data-ttu-id="33fc3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33fc3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

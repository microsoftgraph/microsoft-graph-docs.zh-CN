---
title: 列出存储桶
description: 检索 **plannerbucket** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 155fb4b331f7f78388c3811021bb675de11f3b14
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049469"
---
# <a name="list-buckets"></a><span data-ttu-id="cca9e-103">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="cca9e-103">List buckets</span></span>

<span data-ttu-id="cca9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cca9e-105">检索 **plannerbucket** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cca9e-105">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cca9e-106">权限</span><span class="sxs-lookup"><span data-stu-id="cca9e-106">Permissions</span></span>
<span data-ttu-id="cca9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cca9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cca9e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cca9e-109">Permission type</span></span>      | <span data-ttu-id="cca9e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cca9e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cca9e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cca9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cca9e-112">任务.读取，任务.ReadWrite，Group.Read.All，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca9e-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cca9e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cca9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca9e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cca9e-114">Not supported.</span></span>    |
|<span data-ttu-id="cca9e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cca9e-115">Application</span></span> | <span data-ttu-id="cca9e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cca9e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cca9e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cca9e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cca9e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cca9e-118">Optional query parameters</span></span>
<span data-ttu-id="cca9e-119">此方法要求指定 planId [筛选器](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cca9e-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cca9e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cca9e-120">Request headers</span></span>
| <span data-ttu-id="cca9e-121">名称</span><span class="sxs-lookup"><span data-stu-id="cca9e-121">Name</span></span>      |<span data-ttu-id="cca9e-122">说明</span><span class="sxs-lookup"><span data-stu-id="cca9e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cca9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cca9e-123">Authorization</span></span>  | <span data-ttu-id="cca9e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cca9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cca9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cca9e-126">Request body</span></span>
<span data-ttu-id="cca9e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cca9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca9e-128">响应</span><span class="sxs-lookup"><span data-stu-id="cca9e-128">Response</span></span>

<span data-ttu-id="cca9e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cca9e-129">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="cca9e-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="cca9e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="cca9e-133">示例</span><span class="sxs-lookup"><span data-stu-id="cca9e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cca9e-134">请求</span><span class="sxs-lookup"><span data-stu-id="cca9e-134">Request</span></span>
<span data-ttu-id="cca9e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cca9e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cca9e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cca9e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/buckets
```
# <a name="c"></a>[<span data-ttu-id="cca9e-137">C#</span><span class="sxs-lookup"><span data-stu-id="cca9e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cca9e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cca9e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cca9e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cca9e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cca9e-140">Java</span><span class="sxs-lookup"><span data-stu-id="cca9e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cca9e-141">响应</span><span class="sxs-lookup"><span data-stu-id="cca9e-141">Response</span></span>
<span data-ttu-id="cca9e-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cca9e-142">Here is an example of the response.</span></span> <span data-ttu-id="cca9e-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cca9e-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

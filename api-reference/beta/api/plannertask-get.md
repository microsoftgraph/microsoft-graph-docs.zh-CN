---
title: 获取 plannerTask
description: 检索 **plannertask** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d7b6500ae85214f6eb6608f8ebba14632346fa76
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049987"
---
# <a name="get-plannertask"></a><span data-ttu-id="5be3a-103">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="5be3a-103">Get plannerTask</span></span>

<span data-ttu-id="5be3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5be3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5be3a-105">检索 **plannertask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5be3a-105">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5be3a-106">权限</span><span class="sxs-lookup"><span data-stu-id="5be3a-106">Permissions</span></span>
<span data-ttu-id="5be3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5be3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5be3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5be3a-109">Permission type</span></span>      | <span data-ttu-id="5be3a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5be3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5be3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5be3a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5be3a-112">任务.读取，任务.ReadWrite，Group.Read.All，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5be3a-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5be3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5be3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5be3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5be3a-114">Not supported.</span></span>    |
|<span data-ttu-id="5be3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5be3a-115">Application</span></span> | <span data-ttu-id="5be3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5be3a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5be3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5be3a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5be3a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5be3a-118">Request headers</span></span>
| <span data-ttu-id="5be3a-119">名称</span><span class="sxs-lookup"><span data-stu-id="5be3a-119">Name</span></span>      |<span data-ttu-id="5be3a-120">说明</span><span class="sxs-lookup"><span data-stu-id="5be3a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5be3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5be3a-121">Authorization</span></span>  | <span data-ttu-id="5be3a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5be3a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5be3a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5be3a-124">Request body</span></span>
<span data-ttu-id="5be3a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5be3a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5be3a-126">响应</span><span class="sxs-lookup"><span data-stu-id="5be3a-126">Response</span></span>

<span data-ttu-id="5be3a-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5be3a-127">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="5be3a-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="5be3a-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5be3a-131">示例</span><span class="sxs-lookup"><span data-stu-id="5be3a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5be3a-132">请求</span><span class="sxs-lookup"><span data-stu-id="5be3a-132">Request</span></span>
<span data-ttu-id="5be3a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5be3a-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5be3a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5be3a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
```
# <a name="c"></a>[<span data-ttu-id="5be3a-135">C#</span><span class="sxs-lookup"><span data-stu-id="5be3a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5be3a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5be3a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5be3a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5be3a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5be3a-138">Java</span><span class="sxs-lookup"><span data-stu-id="5be3a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5be3a-139">响应</span><span class="sxs-lookup"><span data-stu-id="5be3a-139">Response</span></span>
<span data-ttu-id="5be3a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5be3a-140">Here is an example of the response.</span></span> <span data-ttu-id="5be3a-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5be3a-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



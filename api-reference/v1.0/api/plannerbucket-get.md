---
title: 获取 plannerBucket
description: 检索 **plannerBucket** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 60d4ea879f7bd430b18d9ad360df9d172b792644
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510947"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="b9389-103">获取 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b9389-103">Get plannerBucket</span></span>

<span data-ttu-id="b9389-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9389-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9389-105">检索 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9389-105">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9389-106">权限</span><span class="sxs-lookup"><span data-stu-id="b9389-106">Permissions</span></span>
<span data-ttu-id="b9389-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9389-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9389-109">Permission type</span></span>      | <span data-ttu-id="b9389-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9389-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9389-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9389-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9389-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9389-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9389-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9389-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9389-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9389-114">Not supported.</span></span>    |
|<span data-ttu-id="b9389-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9389-115">Application</span></span> | <span data-ttu-id="b9389-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9389-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9389-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9389-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9389-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9389-118">Request headers</span></span>
| <span data-ttu-id="b9389-119">名称</span><span class="sxs-lookup"><span data-stu-id="b9389-119">Name</span></span>      |<span data-ttu-id="b9389-120">说明</span><span class="sxs-lookup"><span data-stu-id="b9389-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9389-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9389-121">Authorization</span></span>  | <span data-ttu-id="b9389-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9389-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9389-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9389-124">Request body</span></span>
<span data-ttu-id="b9389-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9389-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9389-126">响应</span><span class="sxs-lookup"><span data-stu-id="b9389-126">Response</span></span>

<span data-ttu-id="b9389-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9389-127">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="b9389-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b9389-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b9389-131">示例</span><span class="sxs-lookup"><span data-stu-id="b9389-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9389-132">请求</span><span class="sxs-lookup"><span data-stu-id="b9389-132">Request</span></span>
<span data-ttu-id="b9389-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9389-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9389-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9389-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
# <a name="c"></a>[<span data-ttu-id="b9389-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9389-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9389-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9389-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9389-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9389-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9389-138">Java</span><span class="sxs-lookup"><span data-stu-id="b9389-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9389-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9389-139">Response</span></span>
<span data-ttu-id="b9389-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9389-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: 创建 plannerBucket
description: 使用此 API 新建 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e59c40b53a9e7e0ab4b06d539330fd61f12b1ae5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510989"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="64b09-103">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="64b09-103">Create plannerBucket</span></span>

<span data-ttu-id="64b09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b09-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64b09-105">使用此 API 新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="64b09-105">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="64b09-106">权限</span><span class="sxs-lookup"><span data-stu-id="64b09-106">Permissions</span></span>
<span data-ttu-id="64b09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64b09-109">Permission type</span></span>      | <span data-ttu-id="64b09-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64b09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64b09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64b09-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64b09-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b09-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64b09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64b09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b09-114">Not supported.</span></span>    |
|<span data-ttu-id="64b09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64b09-115">Application</span></span> | <span data-ttu-id="64b09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b09-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64b09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64b09-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="64b09-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="64b09-118">Request headers</span></span>
| <span data-ttu-id="64b09-119">名称</span><span class="sxs-lookup"><span data-stu-id="64b09-119">Name</span></span>       | <span data-ttu-id="64b09-120">说明</span><span class="sxs-lookup"><span data-stu-id="64b09-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64b09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b09-121">Authorization</span></span>  | <span data-ttu-id="64b09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64b09-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64b09-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="64b09-124">Request body</span></span>
<span data-ttu-id="64b09-125">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b09-125">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64b09-126">响应</span><span class="sxs-lookup"><span data-stu-id="64b09-126">Response</span></span>

<span data-ttu-id="64b09-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64b09-127">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="64b09-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="64b09-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="64b09-131">示例</span><span class="sxs-lookup"><span data-stu-id="64b09-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64b09-132">请求</span><span class="sxs-lookup"><span data-stu-id="64b09-132">Request</span></span>
<span data-ttu-id="64b09-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64b09-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64b09-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="64b09-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="c"></a>[<span data-ttu-id="64b09-135">C#</span><span class="sxs-lookup"><span data-stu-id="64b09-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64b09-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64b09-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64b09-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64b09-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64b09-138">Java</span><span class="sxs-lookup"><span data-stu-id="64b09-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="64b09-139">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b09-139">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="64b09-140">响应</span><span class="sxs-lookup"><span data-stu-id="64b09-140">Response</span></span>
<span data-ttu-id="64b09-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64b09-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

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
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

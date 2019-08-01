---
title: 创建 plannerBucket
description: 使用此 API 新建 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 397810c3590b9cd0feb1223e8a484bbf175ca266
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976206"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="01756-103">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="01756-103">Create plannerBucket</span></span>

<span data-ttu-id="01756-104">使用此 API 新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="01756-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="01756-105">权限</span><span class="sxs-lookup"><span data-stu-id="01756-105">Permissions</span></span>
<span data-ttu-id="01756-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01756-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="01756-108">Permission type</span></span>      | <span data-ttu-id="01756-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01756-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01756-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01756-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01756-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01756-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01756-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01756-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01756-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01756-113">Not supported.</span></span>    |
|<span data-ttu-id="01756-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="01756-114">Application</span></span> | <span data-ttu-id="01756-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01756-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01756-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01756-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="01756-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="01756-117">Request headers</span></span>
| <span data-ttu-id="01756-118">名称</span><span class="sxs-lookup"><span data-stu-id="01756-118">Name</span></span>       | <span data-ttu-id="01756-119">说明</span><span class="sxs-lookup"><span data-stu-id="01756-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01756-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="01756-120">Authorization</span></span>  | <span data-ttu-id="01756-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01756-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01756-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="01756-123">Request body</span></span>
<span data-ttu-id="01756-124">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01756-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="01756-125">响应</span><span class="sxs-lookup"><span data-stu-id="01756-125">Response</span></span>

<span data-ttu-id="01756-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01756-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="01756-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="01756-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="01756-130">示例</span><span class="sxs-lookup"><span data-stu-id="01756-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01756-131">请求</span><span class="sxs-lookup"><span data-stu-id="01756-131">Request</span></span>
<span data-ttu-id="01756-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01756-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01756-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="01756-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="01756-134">C#</span><span class="sxs-lookup"><span data-stu-id="01756-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01756-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="01756-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01756-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="01756-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="01756-137">Java</span><span class="sxs-lookup"><span data-stu-id="01756-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="01756-138">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01756-138">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="01756-139">响应</span><span class="sxs-lookup"><span data-stu-id="01756-139">Response</span></span>
<span data-ttu-id="01756-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01756-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

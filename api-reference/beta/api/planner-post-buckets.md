---
title: 创建 plannerBucket
description: 使用此 API 新建 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b04dd3337f07930e8abd893bb34ea52937199146
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413536"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="13ebd-103">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="13ebd-103">Create plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13ebd-104">使用此 API 新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="13ebd-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="13ebd-105">权限</span><span class="sxs-lookup"><span data-stu-id="13ebd-105">Permissions</span></span>
<span data-ttu-id="13ebd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13ebd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="13ebd-108">Permission type</span></span>      | <span data-ttu-id="13ebd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13ebd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13ebd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13ebd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13ebd-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ebd-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="13ebd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13ebd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13ebd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="13ebd-113">Not supported.</span></span>    |
|<span data-ttu-id="13ebd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="13ebd-114">Application</span></span> | <span data-ttu-id="13ebd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13ebd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13ebd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13ebd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="13ebd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="13ebd-117">Request headers</span></span>
| <span data-ttu-id="13ebd-118">名称</span><span class="sxs-lookup"><span data-stu-id="13ebd-118">Name</span></span>       | <span data-ttu-id="13ebd-119">说明</span><span class="sxs-lookup"><span data-stu-id="13ebd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13ebd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="13ebd-120">Authorization</span></span>  | <span data-ttu-id="13ebd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13ebd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13ebd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="13ebd-123">Request body</span></span>
<span data-ttu-id="13ebd-124">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13ebd-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="13ebd-125">响应</span><span class="sxs-lookup"><span data-stu-id="13ebd-125">Response</span></span>

<span data-ttu-id="13ebd-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13ebd-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="13ebd-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="13ebd-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="13ebd-130">示例</span><span class="sxs-lookup"><span data-stu-id="13ebd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13ebd-131">请求</span><span class="sxs-lookup"><span data-stu-id="13ebd-131">Request</span></span>
<span data-ttu-id="13ebd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13ebd-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13ebd-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="13ebd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13ebd-134">C#</span><span class="sxs-lookup"><span data-stu-id="13ebd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13ebd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13ebd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13ebd-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="13ebd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="13ebd-137">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13ebd-137">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="13ebd-138">响应</span><span class="sxs-lookup"><span data-stu-id="13ebd-138">Response</span></span>
<span data-ttu-id="13ebd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13ebd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

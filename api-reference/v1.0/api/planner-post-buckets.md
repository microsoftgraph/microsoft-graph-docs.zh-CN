---
title: 创建 plannerBucket
description: 使用此 API 新建 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5d642779f7ca179a6de485fae2caaafd065c050d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948350"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="b2cba-103">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b2cba-103">Create plannerBucket</span></span>

<span data-ttu-id="b2cba-104">使用此 API 新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="b2cba-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2cba-105">权限</span><span class="sxs-lookup"><span data-stu-id="b2cba-105">Permissions</span></span>
<span data-ttu-id="b2cba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2cba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2cba-108">Permission type</span></span>      | <span data-ttu-id="b2cba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2cba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2cba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2cba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2cba-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cba-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2cba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2cba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2cba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2cba-113">Not supported.</span></span>    |
|<span data-ttu-id="b2cba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2cba-114">Application</span></span> | <span data-ttu-id="b2cba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2cba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2cba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2cba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="b2cba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2cba-117">Request headers</span></span>
| <span data-ttu-id="b2cba-118">名称</span><span class="sxs-lookup"><span data-stu-id="b2cba-118">Name</span></span>       | <span data-ttu-id="b2cba-119">说明</span><span class="sxs-lookup"><span data-stu-id="b2cba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2cba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2cba-120">Authorization</span></span>  | <span data-ttu-id="b2cba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2cba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2cba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2cba-123">Request body</span></span>
<span data-ttu-id="b2cba-124">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2cba-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b2cba-125">响应</span><span class="sxs-lookup"><span data-stu-id="b2cba-125">Response</span></span>

<span data-ttu-id="b2cba-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2cba-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="b2cba-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b2cba-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b2cba-130">示例</span><span class="sxs-lookup"><span data-stu-id="b2cba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2cba-131">请求</span><span class="sxs-lookup"><span data-stu-id="b2cba-131">Request</span></span>
<span data-ttu-id="b2cba-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2cba-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="b2cba-133">在请求正文中，提供 [plannerBucket](../resources/plannerbucket.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2cba-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b2cba-134">响应</span><span class="sxs-lookup"><span data-stu-id="b2cba-134">Response</span></span>
<span data-ttu-id="b2cba-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2cba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->

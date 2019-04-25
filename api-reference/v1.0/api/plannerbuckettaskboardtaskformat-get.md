---
title: 获取 plannerBucketTaskBoardTaskFormat
description: 检索 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e713786f75e883e58a861256b599089380752af5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562011"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="6f65d-103">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6f65d-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="6f65d-104">检索 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f65d-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f65d-105">权限</span><span class="sxs-lookup"><span data-stu-id="6f65d-105">Permissions</span></span>
<span data-ttu-id="6f65d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f65d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f65d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f65d-108">Permission type</span></span>      | <span data-ttu-id="6f65d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f65d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f65d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f65d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f65d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f65d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f65d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f65d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f65d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f65d-113">Not supported.</span></span>    |
|<span data-ttu-id="6f65d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f65d-114">Application</span></span> | <span data-ttu-id="6f65d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f65d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f65d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f65d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="6f65d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f65d-117">Request headers</span></span>
| <span data-ttu-id="6f65d-118">名称</span><span class="sxs-lookup"><span data-stu-id="6f65d-118">Name</span></span>      |<span data-ttu-id="6f65d-119">说明</span><span class="sxs-lookup"><span data-stu-id="6f65d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f65d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f65d-120">Authorization</span></span>  | <span data-ttu-id="6f65d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f65d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f65d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f65d-123">Request body</span></span>
<span data-ttu-id="6f65d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f65d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f65d-125">响应</span><span class="sxs-lookup"><span data-stu-id="6f65d-125">Response</span></span>

<span data-ttu-id="6f65d-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f65d-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="6f65d-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="6f65d-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6f65d-130">示例</span><span class="sxs-lookup"><span data-stu-id="6f65d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f65d-131">请求</span><span class="sxs-lookup"><span data-stu-id="6f65d-131">Request</span></span>
<span data-ttu-id="6f65d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f65d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="6f65d-133">响应</span><span class="sxs-lookup"><span data-stu-id="6f65d-133">Response</span></span>
<span data-ttu-id="6f65d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f65d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

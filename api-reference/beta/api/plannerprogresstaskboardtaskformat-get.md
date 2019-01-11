---
title: 获取 plannerProgressTaskBoardTaskFormat
description: 检索 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 710ee7ff46c78e18318232e0aa0e4a9d9e86f57f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830392"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="5a22e-103">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5a22e-103">Get plannerProgressTaskBoardTaskFormat</span></span>

> <span data-ttu-id="5a22e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a22e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a22e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a22e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a22e-106">检索 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a22e-106">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a22e-107">权限</span><span class="sxs-lookup"><span data-stu-id="5a22e-107">Permissions</span></span>
<span data-ttu-id="5a22e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a22e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a22e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a22e-110">Permission type</span></span>      | <span data-ttu-id="5a22e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a22e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a22e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a22e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a22e-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a22e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a22e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a22e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a22e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a22e-115">Not supported.</span></span>    |
|<span data-ttu-id="5a22e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a22e-116">Application</span></span> | <span data-ttu-id="5a22e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a22e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a22e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a22e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="5a22e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a22e-119">Request headers</span></span>
| <span data-ttu-id="5a22e-120">名称</span><span class="sxs-lookup"><span data-stu-id="5a22e-120">Name</span></span>      |<span data-ttu-id="5a22e-121">说明</span><span class="sxs-lookup"><span data-stu-id="5a22e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a22e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a22e-122">Authorization</span></span>  | <span data-ttu-id="5a22e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a22e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a22e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a22e-125">Request body</span></span>
<span data-ttu-id="5a22e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a22e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a22e-127">响应</span><span class="sxs-lookup"><span data-stu-id="5a22e-127">Response</span></span>

<span data-ttu-id="5a22e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a22e-128">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="5a22e-p104">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="5a22e-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5a22e-132">示例</span><span class="sxs-lookup"><span data-stu-id="5a22e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a22e-133">请求</span><span class="sxs-lookup"><span data-stu-id="5a22e-133">Request</span></span>
<span data-ttu-id="5a22e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a22e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="5a22e-135">响应</span><span class="sxs-lookup"><span data-stu-id="5a22e-135">Response</span></span>
<span data-ttu-id="5a22e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a22e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 获取 plannerAssignedToTaskBoardTaskFormat
description: 检索 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eed81ce74d7e90ba19e90d9d4280686f5716c73e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963456"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="00580-103">获取 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="00580-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="00580-104">检索 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00580-104">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00580-105">权限</span><span class="sxs-lookup"><span data-stu-id="00580-105">Permissions</span></span>
<span data-ttu-id="00580-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00580-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="00580-108">Permission type</span></span>      | <span data-ttu-id="00580-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00580-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00580-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00580-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00580-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00580-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="00580-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00580-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00580-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="00580-113">Not supported.</span></span>    |
|<span data-ttu-id="00580-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="00580-114">Application</span></span> | <span data-ttu-id="00580-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00580-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00580-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00580-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="00580-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00580-117">Request headers</span></span>
| <span data-ttu-id="00580-118">名称</span><span class="sxs-lookup"><span data-stu-id="00580-118">Name</span></span>      |<span data-ttu-id="00580-119">说明</span><span class="sxs-lookup"><span data-stu-id="00580-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00580-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00580-120">Authorization</span></span>  | <span data-ttu-id="00580-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00580-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00580-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="00580-123">Request body</span></span>
<span data-ttu-id="00580-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00580-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00580-125">响应</span><span class="sxs-lookup"><span data-stu-id="00580-125">Response</span></span>

<span data-ttu-id="00580-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00580-126">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="00580-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="00580-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="00580-130">示例</span><span class="sxs-lookup"><span data-stu-id="00580-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00580-131">请求</span><span class="sxs-lookup"><span data-stu-id="00580-131">Request</span></span>
<span data-ttu-id="00580-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00580-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="00580-133">响应</span><span class="sxs-lookup"><span data-stu-id="00580-133">Response</span></span>
<span data-ttu-id="00580-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00580-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

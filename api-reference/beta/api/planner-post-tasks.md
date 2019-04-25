---
title: 创建 plannerTask
description: 使用此 API 新建 **plannerTask**。
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f74e41e3c855fd6cf54019e2cfd13e36fce45b7e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538943"
---
# <a name="create-plannertask"></a><span data-ttu-id="e6998-103">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="e6998-103">Create plannerTask</span></span>

<span data-ttu-id="e6998-104">使用此 API 新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="e6998-104">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6998-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6998-105">Permissions</span></span>
<span data-ttu-id="e6998-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6998-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6998-108">Permission type</span></span>      | <span data-ttu-id="e6998-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6998-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6998-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6998-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6998-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6998-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e6998-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6998-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6998-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6998-113">Not supported.</span></span>    |
|<span data-ttu-id="e6998-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6998-114">Application</span></span> | <span data-ttu-id="e6998-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6998-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6998-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6998-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="e6998-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6998-117">Request headers</span></span>
| <span data-ttu-id="e6998-118">名称</span><span class="sxs-lookup"><span data-stu-id="e6998-118">Name</span></span>       | <span data-ttu-id="e6998-119">说明</span><span class="sxs-lookup"><span data-stu-id="e6998-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6998-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6998-120">Authorization</span></span>  | <span data-ttu-id="e6998-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6998-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6998-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6998-123">Request body</span></span>
<span data-ttu-id="e6998-p103">在请求正文中，提供 [plannerTask](../resources/plannertask.md) 对象的 JSON 表示形式。**plannerTask** planId 属性必须设为现有的 [plannerPlan](../resources/plannerplan.md) 对象的 id。</span><span class="sxs-lookup"><span data-stu-id="e6998-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="e6998-126">响应</span><span class="sxs-lookup"><span data-stu-id="e6998-126">Response</span></span>

<span data-ttu-id="e6998-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6998-127">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="e6998-p104">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="e6998-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e6998-131">示例</span><span class="sxs-lookup"><span data-stu-id="e6998-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6998-132">请求</span><span class="sxs-lookup"><span data-stu-id="e6998-132">Request</span></span>
<span data-ttu-id="e6998-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6998-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  },
}
```
<span data-ttu-id="e6998-134">在请求正文中，提供 [plannerTask](../resources/plannertask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6998-134">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6998-135">响应</span><span class="sxs-lookup"><span data-stu-id="e6998-135">Response</span></span>
<span data-ttu-id="e6998-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6998-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

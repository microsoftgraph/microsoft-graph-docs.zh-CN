---
title: 创建 plannerTask
description: 使用此 API 新建 **plannerTask**。
ms.openlocfilehash: ca810679ad019b11697f190b3c218c7ee8de42c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042094"
---
# <a name="create-plannertask"></a><span data-ttu-id="4076a-103">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="4076a-103">Create plannerTask</span></span>

> <span data-ttu-id="4076a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4076a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4076a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4076a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4076a-106">使用此 API 新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="4076a-106">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="4076a-107">权限</span><span class="sxs-lookup"><span data-stu-id="4076a-107">Permissions</span></span>
<span data-ttu-id="4076a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4076a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4076a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4076a-110">Permission type</span></span>      | <span data-ttu-id="4076a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4076a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4076a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4076a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4076a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4076a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4076a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4076a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4076a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4076a-115">Not supported.</span></span>    |
|<span data-ttu-id="4076a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4076a-116">Application</span></span> | <span data-ttu-id="4076a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4076a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4076a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4076a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="4076a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4076a-119">Request headers</span></span>
| <span data-ttu-id="4076a-120">名称</span><span class="sxs-lookup"><span data-stu-id="4076a-120">Name</span></span>       | <span data-ttu-id="4076a-121">说明</span><span class="sxs-lookup"><span data-stu-id="4076a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4076a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4076a-122">Authorization</span></span>  | <span data-ttu-id="4076a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4076a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4076a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4076a-125">Request body</span></span>
<span data-ttu-id="4076a-p104">在请求正文中，提供 [plannerTask](../resources/plannertask.md) 对象的 JSON 表示形式。**plannerTask** planId 属性必须设为现有的 [plannerPlan](../resources/plannerplan.md) 对象的 id。</span><span class="sxs-lookup"><span data-stu-id="4076a-p104">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="4076a-128">响应</span><span class="sxs-lookup"><span data-stu-id="4076a-128">Response</span></span>

<span data-ttu-id="4076a-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4076a-129">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="4076a-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4076a-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4076a-133">示例</span><span class="sxs-lookup"><span data-stu-id="4076a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4076a-134">请求</span><span class="sxs-lookup"><span data-stu-id="4076a-134">Request</span></span>
<span data-ttu-id="4076a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4076a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/tasks
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
<span data-ttu-id="4076a-136">在请求正文中，提供 [plannerTask](../resources/plannertask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4076a-136">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4076a-137">响应</span><span class="sxs-lookup"><span data-stu-id="4076a-137">Response</span></span>
<span data-ttu-id="4076a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4076a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
---
title: 列出任务
description: 检索分配给用户的 **plannertask** 对象的列表。
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ff391b31aa82daf8f1080938ad6555090e7e3d96
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967985"
---
# <a name="list-tasks"></a><span data-ttu-id="63321-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="63321-103">List tasks</span></span>

<span data-ttu-id="63321-104">检索分配给用户的 **plannertask** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="63321-104">Retrieve a list of **plannertask** objects assigned to a User.</span></span>
## <a name="permissions"></a><span data-ttu-id="63321-105">权限</span><span class="sxs-lookup"><span data-stu-id="63321-105">Permissions</span></span>
<span data-ttu-id="63321-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63321-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63321-108">Permission type</span></span>      | <span data-ttu-id="63321-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63321-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63321-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63321-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63321-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63321-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63321-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63321-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63321-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="63321-113">Not supported.</span></span>    |
|<span data-ttu-id="63321-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63321-114">Application</span></span> | <span data-ttu-id="63321-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63321-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63321-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63321-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/tasks
GET /users/{id}/planner/tasks
GET /drive/root/createdByUser/planner/tasks
```

## <a name="request-headers"></a><span data-ttu-id="63321-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="63321-117">Request headers</span></span>
| <span data-ttu-id="63321-118">名称</span><span class="sxs-lookup"><span data-stu-id="63321-118">Name</span></span>      |<span data-ttu-id="63321-119">说明</span><span class="sxs-lookup"><span data-stu-id="63321-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63321-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="63321-120">Authorization</span></span>  | <span data-ttu-id="63321-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63321-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63321-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="63321-123">Request body</span></span>
<span data-ttu-id="63321-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63321-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63321-125">响应</span><span class="sxs-lookup"><span data-stu-id="63321-125">Response</span></span>

<span data-ttu-id="63321-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerTask](../resources/plannertask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="63321-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="63321-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="63321-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="63321-130">示例</span><span class="sxs-lookup"><span data-stu-id="63321-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63321-131">请求</span><span class="sxs-lookup"><span data-stu-id="63321-131">Request</span></span>
<span data-ttu-id="63321-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63321-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="63321-133">响应</span><span class="sxs-lookup"><span data-stu-id="63321-133">Response</span></span>
<span data-ttu-id="63321-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63321-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

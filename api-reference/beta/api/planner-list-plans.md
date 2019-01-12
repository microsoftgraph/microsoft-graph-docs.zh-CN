---
title: 列出计划
description: 检索 **plannerplan** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9b6a8639957196e0dc5acfed861743a74e5750c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943436"
---
# <a name="list-plans"></a><span data-ttu-id="c4674-103">列出计划</span><span class="sxs-lookup"><span data-stu-id="c4674-103">List plans</span></span>

> <span data-ttu-id="c4674-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c4674-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4674-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c4674-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4674-106">检索 **plannerplan** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c4674-106">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4674-107">权限</span><span class="sxs-lookup"><span data-stu-id="c4674-107">Permissions</span></span>
<span data-ttu-id="c4674-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4674-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4674-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4674-110">Permission type</span></span>      | <span data-ttu-id="c4674-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4674-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4674-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4674-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4674-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4674-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4674-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4674-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4674-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4674-115">Not supported.</span></span>    |
|<span data-ttu-id="c4674-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4674-116">Application</span></span> | <span data-ttu-id="c4674-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4674-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4674-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4674-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4674-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4674-119">Optional query parameters</span></span>
<span data-ttu-id="c4674-120">此方法要求指定所有者[筛选器](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="c4674-120">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4674-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4674-121">Request headers</span></span>
| <span data-ttu-id="c4674-122">名称</span><span class="sxs-lookup"><span data-stu-id="c4674-122">Name</span></span>      |<span data-ttu-id="c4674-123">说明</span><span class="sxs-lookup"><span data-stu-id="c4674-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4674-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4674-124">Authorization</span></span>  | <span data-ttu-id="c4674-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4674-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4674-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4674-127">Request body</span></span>
<span data-ttu-id="c4674-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4674-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4674-129">响应</span><span class="sxs-lookup"><span data-stu-id="c4674-129">Response</span></span>

<span data-ttu-id="c4674-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4674-130">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="c4674-p104">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="c4674-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c4674-134">示例</span><span class="sxs-lookup"><span data-stu-id="c4674-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4674-135">请求</span><span class="sxs-lookup"><span data-stu-id="c4674-135">Request</span></span>
<span data-ttu-id="c4674-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4674-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans
```
##### <a name="response"></a><span data-ttu-id="c4674-137">响应</span><span class="sxs-lookup"><span data-stu-id="c4674-137">Response</span></span>
<span data-ttu-id="c4674-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4674-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

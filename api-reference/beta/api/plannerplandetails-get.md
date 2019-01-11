---
title: 获取 plannerPlanDetails
description: 检索 **plannerplandetails** 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 096e2092a71545c5008d82305f7c137a911db419
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871993"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="53126-103">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="53126-103">Get plannerPlanDetails</span></span>

> <span data-ttu-id="53126-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53126-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53126-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53126-106">检索 **plannerplandetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53126-106">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53126-107">权限</span><span class="sxs-lookup"><span data-stu-id="53126-107">Permissions</span></span>
<span data-ttu-id="53126-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53126-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53126-110">Permission type</span></span>      | <span data-ttu-id="53126-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53126-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53126-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53126-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53126-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53126-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53126-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53126-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53126-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53126-115">Not supported.</span></span>    |
|<span data-ttu-id="53126-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53126-116">Application</span></span> | <span data-ttu-id="53126-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53126-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53126-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53126-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="53126-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53126-119">Request headers</span></span>
| <span data-ttu-id="53126-120">名称</span><span class="sxs-lookup"><span data-stu-id="53126-120">Name</span></span>      |<span data-ttu-id="53126-121">说明</span><span class="sxs-lookup"><span data-stu-id="53126-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53126-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53126-122">Authorization</span></span>  | <span data-ttu-id="53126-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53126-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53126-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53126-125">Request body</span></span>
<span data-ttu-id="53126-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53126-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53126-127">响应</span><span class="sxs-lookup"><span data-stu-id="53126-127">Response</span></span>

<span data-ttu-id="53126-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53126-128">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="53126-p104">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="53126-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="53126-132">示例</span><span class="sxs-lookup"><span data-stu-id="53126-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53126-133">请求</span><span class="sxs-lookup"><span data-stu-id="53126-133">Request</span></span>
<span data-ttu-id="53126-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53126-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
##### <a name="response"></a><span data-ttu-id="53126-135">响应</span><span class="sxs-lookup"><span data-stu-id="53126-135">Response</span></span>
<span data-ttu-id="53126-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53126-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

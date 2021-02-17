---
title: 列出计划
description: 从计划导航属性获取 plannerPlan 资源。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9b1dec9107ced8754947a7ddeb287d52f75b3d58
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272298"
---
# <a name="list-plans"></a><span data-ttu-id="2f38b-103">列出计划</span><span class="sxs-lookup"><span data-stu-id="2f38b-103">List plans</span></span>
<span data-ttu-id="2f38b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f38b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f38b-105">获取[plannerRoster](../resources/plannerplan.md)包含[的 plannerPlans。](../resources/plannerRoster.md)</span><span class="sxs-lookup"><span data-stu-id="2f38b-105">Get the [plannerPlans](../resources/plannerplan.md) contained by the [plannerRoster](../resources/plannerRoster.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f38b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2f38b-106">Permissions</span></span>
<span data-ttu-id="2f38b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f38b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f38b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f38b-109">Permission type</span></span>|<span data-ttu-id="2f38b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f38b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f38b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f38b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f38b-112">Tasks.Read、Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f38b-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2f38b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f38b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f38b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f38b-114">Not supported.</span></span>|
|<span data-ttu-id="2f38b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f38b-115">Application</span></span>|<span data-ttu-id="2f38b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f38b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f38b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f38b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/plans
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f38b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2f38b-118">Optional query parameters</span></span>
<span data-ttu-id="2f38b-119">此方法仅支持以下 OData 查询参数：</span><span class="sxs-lookup"><span data-stu-id="2f38b-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="2f38b-120">$select</span><span class="sxs-lookup"><span data-stu-id="2f38b-120">$select</span></span>

<span data-ttu-id="2f38b-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2f38b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f38b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f38b-122">Request headers</span></span>
|<span data-ttu-id="2f38b-123">名称</span><span class="sxs-lookup"><span data-stu-id="2f38b-123">Name</span></span>|<span data-ttu-id="2f38b-124">说明</span><span class="sxs-lookup"><span data-stu-id="2f38b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2f38b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f38b-125">Authorization</span></span>|<span data-ttu-id="2f38b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f38b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f38b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f38b-128">Request body</span></span>
<span data-ttu-id="2f38b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f38b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f38b-130">响应</span><span class="sxs-lookup"><span data-stu-id="2f38b-130">Response</span></span>

<span data-ttu-id="2f38b-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2f38b-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f38b-132">示例</span><span class="sxs-lookup"><span data-stu-id="2f38b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f38b-133">请求</span><span class="sxs-lookup"><span data-stu-id="2f38b-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2f38b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f38b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplan"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/plans
```
# <a name="c"></a>[<span data-ttu-id="2f38b-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f38b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f38b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f38b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f38b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f38b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f38b-138">Java</span><span class="sxs-lookup"><span data-stu-id="2f38b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2f38b-139">响应</span><span class="sxs-lookup"><span data-stu-id="2f38b-139">Response</span></span>
<span data-ttu-id="2f38b-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2f38b-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerPlan)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlan",
      "id": "c6442b38-2b38-c644-382b-44c6382b44c6",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "title": "Test plan",
      "container": {
        "@odata.type": "microsoft.graph.plannerPlanContainer",
        "url": "https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965",
        "containerId": "6519868f-868f-6519-8f86-19658f861965",
        "type": "roster"
      }
    }
  ]
}
```


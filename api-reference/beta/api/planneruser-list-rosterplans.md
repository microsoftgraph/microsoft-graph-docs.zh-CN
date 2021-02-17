---
title: 列出 rosterPlans
description: 从 rosterPlans 导航属性获取 plannerPlan 资源。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 199697f7cd3ee050caac983e9822007cdc38a557
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272483"
---
# <a name="list-rosterplans"></a><span data-ttu-id="9b565-103">列出 rosterPlans</span><span class="sxs-lookup"><span data-stu-id="9b565-103">List rosterPlans</span></span>
<span data-ttu-id="9b565-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b565-105">获取 [用户是其中](../resources/plannerplan.md) 一个成员 [的 plannerRosters](../resources/plannerroster.md) 包含的 plannerPlans 列表。</span><span class="sxs-lookup"><span data-stu-id="9b565-105">Get the list of [plannerPlans](../resources/plannerplan.md) that are contained by the [plannerRosters](../resources/plannerroster.md) of which the user is a member.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b565-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9b565-106">Permissions</span></span>
<span data-ttu-id="9b565-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b565-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b565-109">Permission type</span></span>|<span data-ttu-id="9b565-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b565-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b565-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b565-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b565-112">Tasks.Read、Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b565-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9b565-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b565-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b565-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b565-114">Not supported.</span></span>|
|<span data-ttu-id="9b565-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b565-115">Application</span></span>|<span data-ttu-id="9b565-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b565-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b565-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b565-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/planner/rosterPlans
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b565-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b565-118">Optional query parameters</span></span>
<span data-ttu-id="9b565-119">此方法仅支持以下 OData 查询参数：</span><span class="sxs-lookup"><span data-stu-id="9b565-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="9b565-120">$select</span><span class="sxs-lookup"><span data-stu-id="9b565-120">$select</span></span>

<span data-ttu-id="9b565-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9b565-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b565-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b565-122">Request headers</span></span>
|<span data-ttu-id="9b565-123">名称</span><span class="sxs-lookup"><span data-stu-id="9b565-123">Name</span></span>|<span data-ttu-id="9b565-124">说明</span><span class="sxs-lookup"><span data-stu-id="9b565-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9b565-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b565-125">Authorization</span></span>|<span data-ttu-id="9b565-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b565-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b565-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b565-128">Request body</span></span>
<span data-ttu-id="9b565-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b565-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b565-130">响应</span><span class="sxs-lookup"><span data-stu-id="9b565-130">Response</span></span>

<span data-ttu-id="9b565-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9b565-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b565-132">示例</span><span class="sxs-lookup"><span data-stu-id="9b565-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b565-133">请求</span><span class="sxs-lookup"><span data-stu-id="9b565-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b565-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b565-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplan"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/planner/rosterPlans
```
# <a name="c"></a>[<span data-ttu-id="9b565-135">C#</span><span class="sxs-lookup"><span data-stu-id="9b565-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b565-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b565-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b565-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b565-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b565-138">Java</span><span class="sxs-lookup"><span data-stu-id="9b565-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9b565-139">响应</span><span class="sxs-lookup"><span data-stu-id="9b565-139">Response</span></span>
<span data-ttu-id="9b565-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9b565-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        "url": "https://graph.microsoft.com/beta/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "containerId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "type": "roster"
      }
    }
  ]
}
```


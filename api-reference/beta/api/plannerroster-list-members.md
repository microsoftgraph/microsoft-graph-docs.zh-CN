---
title: 列出名单成员
description: 从成员导航属性获取 plannerRosterMember 资源。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9c08f29581b549014544ed1de43f6562efb5066f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272537"
---
# <a name="list-members-of-a-roster"></a><span data-ttu-id="d6764-103">列出名单成员</span><span class="sxs-lookup"><span data-stu-id="d6764-103">List members of a roster</span></span>
<span data-ttu-id="d6764-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6764-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6764-105">从 [plannerRoster 获取 plannerRosterMembers](../resources/plannerrostermember.md) [的列表](../resources/plannerroster.md)。</span><span class="sxs-lookup"><span data-stu-id="d6764-105">Get the list of [plannerRosterMembers](../resources/plannerrostermember.md) from a [plannerRoster](../resources/plannerroster.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6764-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d6764-106">Permissions</span></span>
<span data-ttu-id="d6764-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6764-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6764-109">Permission type</span></span>|<span data-ttu-id="d6764-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6764-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6764-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6764-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6764-112">Tasks.Read、Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6764-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d6764-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6764-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6764-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6764-114">Not supported.</span></span>|
|<span data-ttu-id="d6764-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6764-115">Application</span></span>|<span data-ttu-id="d6764-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6764-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6764-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6764-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6764-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6764-118">Optional query parameters</span></span>
<span data-ttu-id="d6764-119">此方法仅支持以下 OData 查询参数：</span><span class="sxs-lookup"><span data-stu-id="d6764-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="d6764-120">$select</span><span class="sxs-lookup"><span data-stu-id="d6764-120">$select</span></span>

<span data-ttu-id="d6764-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d6764-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6764-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6764-122">Request headers</span></span>
|<span data-ttu-id="d6764-123">名称</span><span class="sxs-lookup"><span data-stu-id="d6764-123">Name</span></span>|<span data-ttu-id="d6764-124">说明</span><span class="sxs-lookup"><span data-stu-id="d6764-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6764-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6764-125">Authorization</span></span>|<span data-ttu-id="d6764-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6764-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6764-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6764-128">Request body</span></span>
<span data-ttu-id="d6764-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6764-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6764-130">响应</span><span class="sxs-lookup"><span data-stu-id="d6764-130">Response</span></span>

<span data-ttu-id="d6764-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [plannerRosterMember](../resources/plannerrostermember.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d6764-131">If successful, this method returns a `200 OK` response code and a collection of [plannerRosterMember](../resources/plannerrostermember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6764-132">示例</span><span class="sxs-lookup"><span data-stu-id="d6764-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6764-133">请求</span><span class="sxs-lookup"><span data-stu-id="d6764-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6764-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6764-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerrostermember"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
```
# <a name="c"></a>[<span data-ttu-id="d6764-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6764-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6764-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6764-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6764-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6764-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6764-138">Java</span><span class="sxs-lookup"><span data-stu-id="d6764-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d6764-139">响应</span><span class="sxs-lookup"><span data-stu-id="d6764-139">Response</span></span>
<span data-ttu-id="d6764-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6764-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerRosterMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerRosterMember",
      "id": "670095cd-95cd-6700-cd95-0067cd950067",
      "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
      "tenantId": "7084c257-c1b7-4286-98b0-20ea7b5c1319",
      "roles": [
      ]
    }
  ]
}
```


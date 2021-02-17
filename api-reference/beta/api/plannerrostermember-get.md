---
title: 获取 plannerRosterMember
description: 读取 plannerRosterMember 对象的属性和关系。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 69ccf29dda22790f33f77458e0537667653b329f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272333"
---
# <a name="get-plannerrostermember"></a><span data-ttu-id="d4b32-103">获取 plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="d4b32-103">Get plannerRosterMember</span></span>
<span data-ttu-id="d4b32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4b32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b32-105">读取 [plannerRosterMember](../resources/plannerrostermember.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4b32-105">Read the properties and relationships of a [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b32-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d4b32-106">Permissions</span></span>
<span data-ttu-id="d4b32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4b32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4b32-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4b32-109">Permission type</span></span>|<span data-ttu-id="d4b32-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4b32-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4b32-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4b32-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4b32-112">Tasks.Read、Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4b32-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d4b32-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4b32-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4b32-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4b32-114">Not supported.</span></span>|
|<span data-ttu-id="d4b32-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4b32-115">Application</span></span>|<span data-ttu-id="d4b32-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4b32-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4b32-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4b32-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/members/{plannerRosterMemberId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4b32-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4b32-118">Optional query parameters</span></span>
<span data-ttu-id="d4b32-119">此方法仅支持以下 OData 查询参数：</span><span class="sxs-lookup"><span data-stu-id="d4b32-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="d4b32-120">$select</span><span class="sxs-lookup"><span data-stu-id="d4b32-120">$select</span></span>

<span data-ttu-id="d4b32-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d4b32-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4b32-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4b32-122">Request headers</span></span>
|<span data-ttu-id="d4b32-123">名称</span><span class="sxs-lookup"><span data-stu-id="d4b32-123">Name</span></span>|<span data-ttu-id="d4b32-124">说明</span><span class="sxs-lookup"><span data-stu-id="d4b32-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4b32-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4b32-125">Authorization</span></span>|<span data-ttu-id="d4b32-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4b32-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b32-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4b32-128">Request body</span></span>
<span data-ttu-id="d4b32-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4b32-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b32-130">响应</span><span class="sxs-lookup"><span data-stu-id="d4b32-130">Response</span></span>

<span data-ttu-id="d4b32-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [plannerRosterMember](../resources/plannerrostermember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4b32-131">If successful, this method returns a `200 OK` response code and a [plannerRosterMember](../resources/plannerrostermember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4b32-132">示例</span><span class="sxs-lookup"><span data-stu-id="d4b32-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4b32-133">请求</span><span class="sxs-lookup"><span data-stu-id="d4b32-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4b32-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b32-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerrostermember"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="d4b32-135">C#</span><span class="sxs-lookup"><span data-stu-id="d4b32-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4b32-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4b32-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4b32-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4b32-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4b32-138">Java</span><span class="sxs-lookup"><span data-stu-id="d4b32-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d4b32-139">响应</span><span class="sxs-lookup"><span data-stu-id="d4b32-139">Response</span></span>
<span data-ttu-id="d4b32-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d4b32-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "tenantId": "7084c257-c1b7-4286-98b0-20ea7b5c1319",
  "roles": [
  ]
}
```


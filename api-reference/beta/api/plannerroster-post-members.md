---
title: 创建 plannerRosterMember
description: 创建新的 plannerRosterMember 对象。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e7dac57941d50ee8b543c53982c216c4c19d5d07
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272425"
---
# <a name="create-plannerrostermember"></a><span data-ttu-id="b2947-103">创建 plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="b2947-103">Create plannerRosterMember</span></span>
<span data-ttu-id="b2947-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2947-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2947-105">向 [plannerRoster 对象添加](../resources/plannerrostermember.md) 成员。</span><span class="sxs-lookup"><span data-stu-id="b2947-105">Add a member to the [plannerRoster](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2947-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b2947-106">Permissions</span></span>
<span data-ttu-id="b2947-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2947-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2947-109">Permission type</span></span>|<span data-ttu-id="b2947-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2947-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2947-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2947-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2947-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2947-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b2947-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2947-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2947-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2947-114">Not supported.</span></span>|
|<span data-ttu-id="b2947-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2947-115">Application</span></span>|<span data-ttu-id="b2947-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2947-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2947-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2947-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters/{plannerRosterId}/members
```

## <a name="request-headers"></a><span data-ttu-id="b2947-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2947-118">Request headers</span></span>
|<span data-ttu-id="b2947-119">名称</span><span class="sxs-lookup"><span data-stu-id="b2947-119">Name</span></span>|<span data-ttu-id="b2947-120">说明</span><span class="sxs-lookup"><span data-stu-id="b2947-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b2947-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2947-121">Authorization</span></span>|<span data-ttu-id="b2947-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2947-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b2947-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2947-124">Content-Type</span></span>|<span data-ttu-id="b2947-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b2947-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2947-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2947-127">Request body</span></span>
<span data-ttu-id="b2947-128">在请求正文中，提供 [plannerRosterMember](../resources/plannerrostermember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2947-128">In the request body, supply a JSON representation of the [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

<span data-ttu-id="b2947-129">下表显示创建 [plannerRosterMember 时所需的属性](../resources/plannerrostermember.md)。</span><span class="sxs-lookup"><span data-stu-id="b2947-129">The following table shows the properties that are required when you create the [plannerRosterMember](../resources/plannerrostermember.md).</span></span>

|<span data-ttu-id="b2947-130">属性</span><span class="sxs-lookup"><span data-stu-id="b2947-130">Property</span></span>|<span data-ttu-id="b2947-131">类型</span><span class="sxs-lookup"><span data-stu-id="b2947-131">Type</span></span>|<span data-ttu-id="b2947-132">描述</span><span class="sxs-lookup"><span data-stu-id="b2947-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2947-133">userId</span><span class="sxs-lookup"><span data-stu-id="b2947-133">userId</span></span>|<span data-ttu-id="b2947-134">String</span><span class="sxs-lookup"><span data-stu-id="b2947-134">String</span></span>|<span data-ttu-id="b2947-135">的标识符。</span><span class="sxs-lookup"><span data-stu-id="b2947-135">Identifier of the .</span></span>|
|<span data-ttu-id="b2947-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="b2947-136">tenantId</span></span>|<span data-ttu-id="b2947-137">String</span><span class="sxs-lookup"><span data-stu-id="b2947-137">String</span></span>|<span data-ttu-id="b2947-138">用户所属的租户的标识符。</span><span class="sxs-lookup"><span data-stu-id="b2947-138">Identifier of the tenant the user belongs to.</span></span> <span data-ttu-id="b2947-139">可选。</span><span class="sxs-lookup"><span data-stu-id="b2947-139">Optional.</span></span> <span data-ttu-id="b2947-140">目前，名单成员不能来自不同的租户。</span><span class="sxs-lookup"><span data-stu-id="b2947-140">Currently roster members cannot be from different tenants.</span></span>|
|<span data-ttu-id="b2947-141">角色</span><span class="sxs-lookup"><span data-stu-id="b2947-141">roles</span></span>|<span data-ttu-id="b2947-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b2947-142">String collection</span></span>|<span data-ttu-id="b2947-143">分配给用户的其他角色。</span><span class="sxs-lookup"><span data-stu-id="b2947-143">Additional roles assigned to the user.</span></span> <span data-ttu-id="b2947-144">可选。</span><span class="sxs-lookup"><span data-stu-id="b2947-144">Optional.</span></span> <span data-ttu-id="b2947-145">当前没有可供用户使用的其他角色。</span><span class="sxs-lookup"><span data-stu-id="b2947-145">Currently there are no additional roles available for users.</span></span>|



## <a name="response"></a><span data-ttu-id="b2947-146">响应</span><span class="sxs-lookup"><span data-stu-id="b2947-146">Response</span></span>

<span data-ttu-id="b2947-147">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [plannerRosterMember](../resources/plannerrostermember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2947-147">If successful, this method returns a `201 Created` response code and a [plannerRosterMember](../resources/plannerrostermember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2947-148">示例</span><span class="sxs-lookup"><span data-stu-id="b2947-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2947-149">请求</span><span class="sxs-lookup"><span data-stu-id="b2947-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b2947-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2947-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerrostermember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
Content-Type: application/json
Content-length: 78

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "userId": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="b2947-151">C#</span><span class="sxs-lookup"><span data-stu-id="b2947-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerrostermember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2947-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2947-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerrostermember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2947-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2947-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerrostermember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2947-154">Java</span><span class="sxs-lookup"><span data-stu-id="b2947-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerrostermember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b2947-155">响应</span><span class="sxs-lookup"><span data-stu-id="b2947-155">Response</span></span>
<span data-ttu-id="b2947-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2947-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "roles": [
  ]
}
```


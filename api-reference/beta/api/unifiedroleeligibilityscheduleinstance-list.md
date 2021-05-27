---
title: 列出 unifiedRoleEligibilityScheduleInstances
description: 获取 unifiedRoleEligibilityScheduleInstance 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c4662d54547beaa1e4af77c204618b5f5a935e29
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680107"
---
# <a name="list-unifiedroleeligibilityscheduleinstances"></a><span data-ttu-id="f9249-103">列出 unifiedRoleEligibilityScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="f9249-103">List unifiedRoleEligibilityScheduleInstances</span></span>
<span data-ttu-id="f9249-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9249-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9249-105">获取 [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="f9249-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9249-106">权限</span><span class="sxs-lookup"><span data-stu-id="f9249-106">Permissions</span></span>
<span data-ttu-id="f9249-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9249-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9249-109">Permission type</span></span>|<span data-ttu-id="f9249-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9249-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9249-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9249-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9249-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f9249-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="f9249-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9249-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9249-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f9249-114">Not supported</span></span>|
|<span data-ttu-id="f9249-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9249-115">Application</span></span>|<span data-ttu-id="f9249-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f9249-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9249-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9249-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9249-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9249-118">Optional query parameters</span></span>
<span data-ttu-id="f9249-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9249-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9249-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f9249-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9249-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9249-121">Request headers</span></span>
|<span data-ttu-id="f9249-122">名称</span><span class="sxs-lookup"><span data-stu-id="f9249-122">Name</span></span>|<span data-ttu-id="f9249-123">说明</span><span class="sxs-lookup"><span data-stu-id="f9249-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9249-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9249-124">Authorization</span></span>|<span data-ttu-id="f9249-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9249-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9249-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9249-127">Request body</span></span>
<span data-ttu-id="f9249-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9249-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9249-129">响应</span><span class="sxs-lookup"><span data-stu-id="f9249-129">Response</span></span>

<span data-ttu-id="f9249-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9249-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9249-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9249-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9249-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9249-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f9249-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9249-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances
```
# <a name="c"></a>[<span data-ttu-id="f9249-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9249-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9249-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9249-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9249-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9249-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9249-137">Java</span><span class="sxs-lookup"><span data-stu-id="f9249-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f9249-138">响应</span><span class="sxs-lookup"><span data-stu-id="f9249-138">Response</span></span>
<span data-ttu-id="f9249-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9249-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "principalId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "roleDefinitionId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "directoryScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "appScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1"
    }
  ]
}
```


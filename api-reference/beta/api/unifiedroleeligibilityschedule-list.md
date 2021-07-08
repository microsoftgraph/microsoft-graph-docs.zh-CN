---
title: 列出 unifiedRoleEligibilitySchedules
description: 获取 unifiedRoleEligibilitySchedule 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1817550be3e4903eba3a62e37ad6353b676a3c7d
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334554"
---
# <a name="list-unifiedroleeligibilityschedules"></a><span data-ttu-id="bd6eb-103">列出 unifiedRoleEligibilitySchedules</span><span class="sxs-lookup"><span data-stu-id="bd6eb-103">List unifiedRoleEligibilitySchedules</span></span>
<span data-ttu-id="bd6eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd6eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6eb-105">获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd6eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd6eb-106">Permissions</span></span>
<span data-ttu-id="bd6eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd6eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd6eb-109">Permission type</span></span>|<span data-ttu-id="bd6eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd6eb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd6eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd6eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd6eb-112">RoleEligibilitySchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleEligibilitySchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="bd6eb-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="bd6eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd6eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd6eb-114">不支持</span><span class="sxs-lookup"><span data-stu-id="bd6eb-114">Not supported</span></span>|
|<span data-ttu-id="bd6eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd6eb-115">Application</span></span>|<span data-ttu-id="bd6eb-116">RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="bd6eb-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd6eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd6eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd6eb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd6eb-118">Optional query parameters</span></span>
<span data-ttu-id="bd6eb-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bd6eb-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd6eb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd6eb-121">Request headers</span></span>
|<span data-ttu-id="bd6eb-122">名称</span><span class="sxs-lookup"><span data-stu-id="bd6eb-122">Name</span></span>|<span data-ttu-id="bd6eb-123">说明</span><span class="sxs-lookup"><span data-stu-id="bd6eb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bd6eb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd6eb-124">Authorization</span></span>|<span data-ttu-id="bd6eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd6eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd6eb-127">Request body</span></span>
<span data-ttu-id="bd6eb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6eb-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd6eb-129">Response</span></span>

<span data-ttu-id="bd6eb-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd6eb-131">示例</span><span class="sxs-lookup"><span data-stu-id="bd6eb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd6eb-132">请求</span><span class="sxs-lookup"><span data-stu-id="bd6eb-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bd6eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules
```
# <a name="c"></a>[<span data-ttu-id="bd6eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="bd6eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd6eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd6eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd6eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd6eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd6eb-137">Java</span><span class="sxs-lookup"><span data-stu-id="bd6eb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bd6eb-138">响应</span><span class="sxs-lookup"><span data-stu-id="bd6eb-138">Response</span></span>
<span data-ttu-id="bd6eb-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd6eb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "memberType": "direct"
    }
  ]
}
```


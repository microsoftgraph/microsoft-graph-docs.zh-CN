---
title: 获取 unifiedRoleManagementPolicy
description: 读取 unifiedRoleManagementPolicy 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 70f4b1d5d59f5306e5b73f08b5385dc96ea8ac9c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682341"
---
# <a name="get-unifiedrolemanagementpolicy"></a><span data-ttu-id="5d3d9-103">获取 unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="5d3d9-103">Get unifiedRoleManagementPolicy</span></span>
<span data-ttu-id="5d3d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3d9-105">读取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-105">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3d9-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d3d9-106">Permissions</span></span>
<span data-ttu-id="5d3d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3d9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d3d9-109">Permission type</span></span>|<span data-ttu-id="5d3d9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d3d9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d3d9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d3d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d3d9-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="5d3d9-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="5d3d9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d3d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d3d9-114">不支持</span><span class="sxs-lookup"><span data-stu-id="5d3d9-114">Not supported</span></span>|
|<span data-ttu-id="5d3d9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d3d9-115">Application</span></span>|<span data-ttu-id="5d3d9-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="5d3d9-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d3d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d3d9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d3d9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5d3d9-118">Optional query parameters</span></span>
<span data-ttu-id="5d3d9-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5d3d9-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d3d9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d3d9-121">Request headers</span></span>
|<span data-ttu-id="5d3d9-122">名称</span><span class="sxs-lookup"><span data-stu-id="5d3d9-122">Name</span></span>|<span data-ttu-id="5d3d9-123">说明</span><span class="sxs-lookup"><span data-stu-id="5d3d9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d3d9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3d9-124">Authorization</span></span>|<span data-ttu-id="5d3d9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d3d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d3d9-127">Request body</span></span>
<span data-ttu-id="5d3d9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3d9-129">响应</span><span class="sxs-lookup"><span data-stu-id="5d3d9-129">Response</span></span>

<span data-ttu-id="5d3d9-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d3d9-131">示例</span><span class="sxs-lookup"><span data-stu-id="5d3d9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d3d9-132">请求</span><span class="sxs-lookup"><span data-stu-id="5d3d9-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d3d9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3d9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9
```
# <a name="c"></a>[<span data-ttu-id="5d3d9-134">C#</span><span class="sxs-lookup"><span data-stu-id="5d3d9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d3d9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d3d9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d3d9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d3d9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d3d9-137">Java</span><span class="sxs-lookup"><span data-stu-id="5d3d9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d3d9-138">响应</span><span class="sxs-lookup"><span data-stu-id="5d3d9-138">Response</span></span>
<span data-ttu-id="5d3d9-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d3d9-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "displayName": "Policy1",
    "description": "Policy for privileged admins",
    "isOrganizationDefault": true,
    "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "scopeType": "subscription",
    "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```


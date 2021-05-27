---
title: 列出 roleManagementPolicies
description: 从 roleManagementPolicies 导航属性获取 unifiedRoleManagementPolicy 资源。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d51e045c25229ceffe84a3553be8878b001bdc24
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680729"
---
# <a name="list-rolemanagementpolicies"></a><span data-ttu-id="ccb9d-103">列出 roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="ccb9d-103">List roleManagementPolicies</span></span>
<span data-ttu-id="ccb9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccb9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="ccb9d-105">从 roleManagementPolicies 导航属性获取 unifiedRoleManagementPolicy 资源。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-105">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>


## <a name="permissions"></a><span data-ttu-id="ccb9d-106">权限</span><span class="sxs-lookup"><span data-stu-id="ccb9d-106">Permissions</span></span>
<span data-ttu-id="ccb9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccb9d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccb9d-109">Permission type</span></span>|<span data-ttu-id="ccb9d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccb9d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccb9d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccb9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccb9d-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ccb9d-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ccb9d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccb9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccb9d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="ccb9d-114">Not supported</span></span>|
|<span data-ttu-id="ccb9d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccb9d-115">Application</span></span>|<span data-ttu-id="ccb9d-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ccb9d-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccb9d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccb9d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccb9d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ccb9d-118">Optional query parameters</span></span>
<span data-ttu-id="ccb9d-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ccb9d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccb9d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccb9d-121">Request headers</span></span>
|<span data-ttu-id="ccb9d-122">名称</span><span class="sxs-lookup"><span data-stu-id="ccb9d-122">Name</span></span>|<span data-ttu-id="ccb9d-123">说明</span><span class="sxs-lookup"><span data-stu-id="ccb9d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ccb9d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccb9d-124">Authorization</span></span>|<span data-ttu-id="ccb9d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccb9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccb9d-127">Request body</span></span>
<span data-ttu-id="ccb9d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccb9d-129">响应</span><span class="sxs-lookup"><span data-stu-id="ccb9d-129">Response</span></span>

<span data-ttu-id="ccb9d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccb9d-131">示例</span><span class="sxs-lookup"><span data-stu-id="ccb9d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccb9d-132">请求</span><span class="sxs-lookup"><span data-stu-id="ccb9d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccb9d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccb9d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies
```
# <a name="c"></a>[<span data-ttu-id="ccb9d-134">C#</span><span class="sxs-lookup"><span data-stu-id="ccb9d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccb9d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccb9d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccb9d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccb9d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccb9d-137">Java</span><span class="sxs-lookup"><span data-stu-id="ccb9d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ccb9d-138">响应</span><span class="sxs-lookup"><span data-stu-id="ccb9d-138">Response</span></span>
<span data-ttu-id="ccb9d-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccb9d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "displayName": "Policy1",
      "description": "A policy for all privileged administrators",
      "isOrganizationDefault": true,
      "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "scopeType": "subscriptions",
      "lastModifiedDateTime": "2021-03-17T02:54:27.167+00:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identity"
      }
    }
  ]
}
```


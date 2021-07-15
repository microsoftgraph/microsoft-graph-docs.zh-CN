---
title: 列出 conditionalAccessPolicyCoverages
description: 获取 conditionalAccessPolicyCoverage 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a35b7032b4b1fb19b73ff4110a4b43af3c388487
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442642"
---
# <a name="list-conditionalaccesspolicycoverages"></a><span data-ttu-id="643ef-103">列出 conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="643ef-103">List conditionalAccessPolicyCoverages</span></span>
<span data-ttu-id="643ef-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="643ef-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="643ef-105">获取 [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="643ef-105">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span> <span data-ttu-id="643ef-106">使用此操作可列出Azure Active Directory多租户管理平台管理的所有租户中的条件访问策略覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="643ef-106">Use this operation to list of Azure Active Directory conditional access policy coverage across all tenants that are being managed by the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="643ef-107">权限</span><span class="sxs-lookup"><span data-stu-id="643ef-107">Permissions</span></span>
<span data-ttu-id="643ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="643ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="643ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="643ef-110">Permission type</span></span>|<span data-ttu-id="643ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="643ef-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="643ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="643ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="643ef-113">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="643ef-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="643ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="643ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="643ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="643ef-115">Not supported.</span></span>|
|<span data-ttu-id="643ef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="643ef-116">Application</span></span>|<span data-ttu-id="643ef-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="643ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="643ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="643ef-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="643ef-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="643ef-119">Optional query parameters</span></span>
<span data-ttu-id="643ef-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="643ef-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="643ef-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="643ef-121">Request headers</span></span>
|<span data-ttu-id="643ef-122">名称</span><span class="sxs-lookup"><span data-stu-id="643ef-122">Name</span></span>|<span data-ttu-id="643ef-123">说明</span><span class="sxs-lookup"><span data-stu-id="643ef-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="643ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="643ef-124">Authorization</span></span>|<span data-ttu-id="643ef-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="643ef-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="643ef-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="643ef-127">Request body</span></span>
<span data-ttu-id="643ef-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="643ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="643ef-129">响应</span><span class="sxs-lookup"><span data-stu-id="643ef-129">Response</span></span>

<span data-ttu-id="643ef-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="643ef-130">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="643ef-131">示例</span><span class="sxs-lookup"><span data-stu-id="643ef-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="643ef-132">请求</span><span class="sxs-lookup"><span data-stu-id="643ef-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="643ef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="643ef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```
# <a name="c"></a>[<span data-ttu-id="643ef-134">C#</span><span class="sxs-lookup"><span data-stu-id="643ef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="643ef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="643ef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="643ef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="643ef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="643ef-137">Java</span><span class="sxs-lookup"><span data-stu-id="643ef-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="643ef-138">响应</span><span class="sxs-lookup"><span data-stu-id="643ef-138">Response</span></span>
><span data-ttu-id="643ef-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="643ef-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.conditionalAccessPolicyCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "conditionalAccessPolicyState": "enabled",
      "requiresDeviceCompliance": false,
      "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```

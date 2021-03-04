---
title: 获取 governanceResource
description: 检索 governanceResource 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 83e41655dd08307f50b0f21f05d9c3b9975de0b2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435985"
---
# <a name="get-governanceresource"></a><span data-ttu-id="b52ad-103">获取 governanceResource</span><span class="sxs-lookup"><span data-stu-id="b52ad-103">Get governanceResource</span></span>

<span data-ttu-id="b52ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52ad-105">检索 [governanceResource 对象的属性和](../resources/governanceresource.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b52ad-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b52ad-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b52ad-106">Permissions</span></span>
<span data-ttu-id="b52ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="b52ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="b52ad-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="b52ad-109">Azure resources</span></span>

| <span data-ttu-id="b52ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b52ad-110">Permission type</span></span> | <span data-ttu-id="b52ad-111">权限</span><span class="sxs-lookup"><span data-stu-id="b52ad-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b52ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b52ad-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b52ad-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b52ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b52ad-115">Not supported.</span></span> |
| <span data-ttu-id="b52ad-116">Application</span><span class="sxs-lookup"><span data-stu-id="b52ad-116">Application</span></span> | <span data-ttu-id="b52ad-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b52ad-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="b52ad-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="b52ad-118">Azure AD</span></span>

| <span data-ttu-id="b52ad-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b52ad-119">Permission type</span></span> | <span data-ttu-id="b52ad-120">权限</span><span class="sxs-lookup"><span data-stu-id="b52ad-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b52ad-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-121">Delegated (work or school account)</span></span> | <span data-ttu-id="b52ad-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b52ad-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="b52ad-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52ad-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b52ad-124">Not supported.</span></span> |
| <span data-ttu-id="b52ad-125">Application</span><span class="sxs-lookup"><span data-stu-id="b52ad-125">Application</span></span> | <span data-ttu-id="b52ad-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b52ad-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="b52ad-127">组</span><span class="sxs-lookup"><span data-stu-id="b52ad-127">Groups</span></span>

|<span data-ttu-id="b52ad-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="b52ad-128">Permission type</span></span> | <span data-ttu-id="b52ad-129">权限</span><span class="sxs-lookup"><span data-stu-id="b52ad-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="b52ad-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b52ad-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b52ad-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="b52ad-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ad-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52ad-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="b52ad-133">Not supported.</span></span> |
| <span data-ttu-id="b52ad-134">Application</span><span class="sxs-lookup"><span data-stu-id="b52ad-134">Application</span></span> | <span data-ttu-id="b52ad-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b52ad-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="b52ad-136">除了权限范围之外，此 API 要求请求者至少对资源角色分配一个权限。</span><span class="sxs-lookup"><span data-stu-id="b52ad-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="b52ad-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b52ad-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b52ad-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b52ad-138">Optional query parameters</span></span>
<span data-ttu-id="b52ad-139">此方法 **仅** 支持  `$select` `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b52ad-139">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b52ad-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="b52ad-140">Request headers</span></span>
| <span data-ttu-id="b52ad-141">名称</span><span class="sxs-lookup"><span data-stu-id="b52ad-141">Name</span></span>      |<span data-ttu-id="b52ad-142">说明</span><span class="sxs-lookup"><span data-stu-id="b52ad-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b52ad-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="b52ad-143">Authorization</span></span>  | <span data-ttu-id="b52ad-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b52ad-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52ad-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="b52ad-145">Request body</span></span>
<span data-ttu-id="b52ad-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b52ad-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b52ad-147">响应</span><span class="sxs-lookup"><span data-stu-id="b52ad-147">Response</span></span>
<span data-ttu-id="b52ad-148">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [governanceResource](../resources/governanceresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b52ad-148">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52ad-149">示例</span><span class="sxs-lookup"><span data-stu-id="b52ad-149">Example</span></span>
<span data-ttu-id="b52ad-150">此示例演示如何获取订阅 Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5) 。</span><span class="sxs-lookup"><span data-stu-id="b52ad-150">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="b52ad-151">请求</span><span class="sxs-lookup"><span data-stu-id="b52ad-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="b52ad-152">响应</span><span class="sxs-lookup"><span data-stu-id="b52ad-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



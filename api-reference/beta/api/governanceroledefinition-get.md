---
title: 获取 governanceRoleDefinition
description: 检索 governanceRoleDefinition 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 97d3ed248d5a808cf57edf5f18cc37cc07e44bf7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435838"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="be885-103">获取 governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="be885-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="be885-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be885-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be885-105">检索 [governanceRoleDefinition 的属性和关系](../resources/governanceroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="be885-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be885-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="be885-106">Permissions</span></span>
<span data-ttu-id="be885-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="be885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="be885-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="be885-109">Azure resources</span></span>

| <span data-ttu-id="be885-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be885-110">Permission type</span></span> | <span data-ttu-id="be885-111">权限</span><span class="sxs-lookup"><span data-stu-id="be885-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="be885-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be885-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="be885-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="be885-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be885-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be885-115">Not supported.</span></span> |
| <span data-ttu-id="be885-116">Application</span><span class="sxs-lookup"><span data-stu-id="be885-116">Application</span></span> | <span data-ttu-id="be885-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="be885-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="be885-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="be885-118">Azure AD</span></span>

| <span data-ttu-id="be885-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="be885-119">Permission type</span></span> | <span data-ttu-id="be885-120">权限</span><span class="sxs-lookup"><span data-stu-id="be885-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="be885-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-121">Delegated (work or school account)</span></span> | <span data-ttu-id="be885-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="be885-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="be885-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be885-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="be885-124">Not supported.</span></span> |
| <span data-ttu-id="be885-125">Application</span><span class="sxs-lookup"><span data-stu-id="be885-125">Application</span></span> | <span data-ttu-id="be885-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="be885-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="be885-127">组</span><span class="sxs-lookup"><span data-stu-id="be885-127">Groups</span></span>

|<span data-ttu-id="be885-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="be885-128">Permission type</span></span> | <span data-ttu-id="be885-129">权限</span><span class="sxs-lookup"><span data-stu-id="be885-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="be885-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-130">Delegated (work or school account)</span></span> | <span data-ttu-id="be885-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="be885-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="be885-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be885-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be885-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="be885-133">Not supported.</span></span> |
| <span data-ttu-id="be885-134">Application</span><span class="sxs-lookup"><span data-stu-id="be885-134">Application</span></span> | <span data-ttu-id="be885-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="be885-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="be885-136">除了权限范围之外，此 API 要求请求者至少角色分配一个 [governanceRoleDefinition](../resources/governanceroledefinition.md) 所属的资源。</span><span class="sxs-lookup"><span data-stu-id="be885-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="be885-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be885-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be885-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be885-138">Optional query parameters</span></span>
<span data-ttu-id="be885-139">此方法 **不支持**[OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be885-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be885-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="be885-140">Request headers</span></span>
| <span data-ttu-id="be885-141">名称</span><span class="sxs-lookup"><span data-stu-id="be885-141">Name</span></span>      |<span data-ttu-id="be885-142">说明</span><span class="sxs-lookup"><span data-stu-id="be885-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be885-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="be885-143">Authorization</span></span>  | <span data-ttu-id="be885-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="be885-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="be885-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="be885-145">Request body</span></span>
<span data-ttu-id="be885-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be885-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be885-147">响应</span><span class="sxs-lookup"><span data-stu-id="be885-147">Response</span></span>
<span data-ttu-id="be885-148">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [governanceRoleDefinition](../resources/governanceroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be885-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be885-149">示例</span><span class="sxs-lookup"><span data-stu-id="be885-149">Example</span></span>
<span data-ttu-id="be885-150">此示例演示如何在订阅 Wingtip Toys - Prod 中获取角色定义 DNS 区域参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="be885-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="be885-151">请求</span><span class="sxs-lookup"><span data-stu-id="be885-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="be885-152">响应</span><span class="sxs-lookup"><span data-stu-id="be885-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



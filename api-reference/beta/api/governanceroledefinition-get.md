---
title: 获取 governanceRoleDefinition
description: 检索 governanceRoleDefinition 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c42eee6a55eed75674f2f53563898dbe9d5e71e7
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350663"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="7d6f1-103">获取 governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d6f1-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="7d6f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d6f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d6f1-105">检索 [governanceRoleDefinition 的属性和关系](../resources/governanceroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d6f1-106">权限</span><span class="sxs-lookup"><span data-stu-id="7d6f1-106">Permissions</span></span>
<span data-ttu-id="7d6f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="7d6f1-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="7d6f1-109">Azure resources</span></span>

| <span data-ttu-id="7d6f1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d6f1-110">Permission type</span></span> | <span data-ttu-id="7d6f1-111">权限</span><span class="sxs-lookup"><span data-stu-id="7d6f1-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7d6f1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d6f1-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7d6f1-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="7d6f1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d6f1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-115">Not supported.</span></span> |
| <span data-ttu-id="7d6f1-116">Application</span><span class="sxs-lookup"><span data-stu-id="7d6f1-116">Application</span></span> | <span data-ttu-id="7d6f1-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7d6f1-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="7d6f1-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="7d6f1-118">Azure AD</span></span>

| <span data-ttu-id="7d6f1-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d6f1-119">Permission type</span></span> | <span data-ttu-id="7d6f1-120">权限</span><span class="sxs-lookup"><span data-stu-id="7d6f1-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7d6f1-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-121">Delegated (work or school account)</span></span> | <span data-ttu-id="7d6f1-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7d6f1-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="7d6f1-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d6f1-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-124">Not supported.</span></span> |
| <span data-ttu-id="7d6f1-125">Application</span><span class="sxs-lookup"><span data-stu-id="7d6f1-125">Application</span></span> | <span data-ttu-id="7d6f1-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7d6f1-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="7d6f1-127">组</span><span class="sxs-lookup"><span data-stu-id="7d6f1-127">Groups</span></span>

|<span data-ttu-id="7d6f1-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d6f1-128">Permission type</span></span> | <span data-ttu-id="7d6f1-129">权限</span><span class="sxs-lookup"><span data-stu-id="7d6f1-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="7d6f1-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-130">Delegated (work or school account)</span></span> | <span data-ttu-id="7d6f1-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="7d6f1-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="7d6f1-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d6f1-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d6f1-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-133">Not supported.</span></span> |
| <span data-ttu-id="7d6f1-134">Application</span><span class="sxs-lookup"><span data-stu-id="7d6f1-134">Application</span></span> | <span data-ttu-id="7d6f1-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="7d6f1-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="7d6f1-136">除了权限范围之外，此 API 要求请求程序对 [governanceRoleDefinition](../resources/governanceroledefinition.md) 所属的资源角色分配至少一个资源。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="7d6f1-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d6f1-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d6f1-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7d6f1-138">Optional query parameters</span></span>
<span data-ttu-id="7d6f1-139">此方法 **不支持**[OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d6f1-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d6f1-140">Request headers</span></span>
| <span data-ttu-id="7d6f1-141">名称</span><span class="sxs-lookup"><span data-stu-id="7d6f1-141">Name</span></span>      |<span data-ttu-id="7d6f1-142">说明</span><span class="sxs-lookup"><span data-stu-id="7d6f1-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d6f1-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d6f1-143">Authorization</span></span>  | <span data-ttu-id="7d6f1-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7d6f1-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="7d6f1-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d6f1-145">Request body</span></span>
<span data-ttu-id="7d6f1-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7d6f1-147">响应</span><span class="sxs-lookup"><span data-stu-id="7d6f1-147">Response</span></span>
<span data-ttu-id="7d6f1-148">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [governanceRoleDefinition](../resources/governanceroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d6f1-149">示例</span><span class="sxs-lookup"><span data-stu-id="7d6f1-149">Example</span></span>
<span data-ttu-id="7d6f1-150">此示例演示如何获取订阅 Wingtip Toys - Prod 中的角色定义 DNS 区域参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7d6f1-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="7d6f1-151">请求</span><span class="sxs-lookup"><span data-stu-id="7d6f1-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="7d6f1-152">响应</span><span class="sxs-lookup"><span data-stu-id="7d6f1-152">Response</span></span>
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



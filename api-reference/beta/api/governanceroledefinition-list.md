---
title: 列出 governanceRoleDefinitions
description: 获取资源上的 governanceRoleDefinitions 集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6e7d6876a9877a1bf8d146086e3aac3ec74ad60d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435810"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="0591c-103">列出 governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="0591c-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="0591c-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0591c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0591c-105">获取资源上的 [governanceRoleDefinitions](../resources/governanceroledefinition.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0591c-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0591c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0591c-106">Permissions</span></span>
<span data-ttu-id="0591c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="0591c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="0591c-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="0591c-109">Azure resources</span></span>

| <span data-ttu-id="0591c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0591c-110">Permission type</span></span> | <span data-ttu-id="0591c-111">权限</span><span class="sxs-lookup"><span data-stu-id="0591c-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0591c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0591c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0591c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="0591c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0591c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0591c-115">Not supported.</span></span> |
| <span data-ttu-id="0591c-116">Application</span><span class="sxs-lookup"><span data-stu-id="0591c-116">Application</span></span> | <span data-ttu-id="0591c-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0591c-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="0591c-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="0591c-118">Azure AD</span></span>

| <span data-ttu-id="0591c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="0591c-119">Permission type</span></span> | <span data-ttu-id="0591c-120">权限</span><span class="sxs-lookup"><span data-stu-id="0591c-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0591c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="0591c-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0591c-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="0591c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0591c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0591c-124">Not supported.</span></span> |
| <span data-ttu-id="0591c-125">Application</span><span class="sxs-lookup"><span data-stu-id="0591c-125">Application</span></span> | <span data-ttu-id="0591c-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0591c-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="0591c-127">组</span><span class="sxs-lookup"><span data-stu-id="0591c-127">Groups</span></span>

|<span data-ttu-id="0591c-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="0591c-128">Permission type</span></span> | <span data-ttu-id="0591c-129">权限</span><span class="sxs-lookup"><span data-stu-id="0591c-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="0591c-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="0591c-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="0591c-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="0591c-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0591c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0591c-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="0591c-133">Not supported.</span></span> |
| <span data-ttu-id="0591c-134">Application</span><span class="sxs-lookup"><span data-stu-id="0591c-134">Application</span></span> | <span data-ttu-id="0591c-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="0591c-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="0591c-136">除了权限范围之外，此 API 要求请求者至少对资源角色分配一个权限。</span><span class="sxs-lookup"><span data-stu-id="0591c-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="0591c-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0591c-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0591c-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0591c-138">Optional query parameters</span></span>
<span data-ttu-id="0591c-139">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0591c-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0591c-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="0591c-140">Request headers</span></span>
| <span data-ttu-id="0591c-141">名称</span><span class="sxs-lookup"><span data-stu-id="0591c-141">Name</span></span>      |<span data-ttu-id="0591c-142">说明</span><span class="sxs-lookup"><span data-stu-id="0591c-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0591c-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="0591c-143">Authorization</span></span>  | <span data-ttu-id="0591c-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0591c-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0591c-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="0591c-145">Request body</span></span>
<span data-ttu-id="0591c-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0591c-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0591c-147">响应</span><span class="sxs-lookup"><span data-stu-id="0591c-147">Response</span></span>
<span data-ttu-id="0591c-148">如果成功，此方法在响应正文中返回 `200 OK` [governanceRoleDefinition](../resources/governanceroledefinition.md) 对象的响应代码和集合。</span><span class="sxs-lookup"><span data-stu-id="0591c-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0591c-149">示例</span><span class="sxs-lookup"><span data-stu-id="0591c-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="0591c-150">此示例演示如何获取订阅 Wingtip Toys - Prod 的所有角色定义。</span><span class="sxs-lookup"><span data-stu-id="0591c-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="0591c-151">请求</span><span class="sxs-lookup"><span data-stu-id="0591c-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="0591c-152">响应</span><span class="sxs-lookup"><span data-stu-id="0591c-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



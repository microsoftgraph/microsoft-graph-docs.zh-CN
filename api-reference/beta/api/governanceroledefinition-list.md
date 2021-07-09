---
title: 列出 governanceRoleDefinitions
description: 获取资源上的 governanceRoleDefinitions 集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7684d3593015d7320c955e4465aacd21c62faae8
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350682"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="066fe-103">列出 governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="066fe-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="066fe-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="066fe-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="066fe-105">获取资源上的 [governanceRoleDefinitions](../resources/governanceroledefinition.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="066fe-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="066fe-106">权限</span><span class="sxs-lookup"><span data-stu-id="066fe-106">Permissions</span></span>
<span data-ttu-id="066fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="066fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="066fe-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="066fe-109">Azure resources</span></span>

| <span data-ttu-id="066fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="066fe-110">Permission type</span></span> | <span data-ttu-id="066fe-111">权限</span><span class="sxs-lookup"><span data-stu-id="066fe-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="066fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="066fe-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="066fe-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="066fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="066fe-115">Not supported.</span></span> |
| <span data-ttu-id="066fe-116">Application</span><span class="sxs-lookup"><span data-stu-id="066fe-116">Application</span></span> | <span data-ttu-id="066fe-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="066fe-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="066fe-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="066fe-118">Azure AD</span></span>

| <span data-ttu-id="066fe-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="066fe-119">Permission type</span></span> | <span data-ttu-id="066fe-120">权限</span><span class="sxs-lookup"><span data-stu-id="066fe-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="066fe-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-121">Delegated (work or school account)</span></span> | <span data-ttu-id="066fe-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="066fe-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="066fe-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066fe-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="066fe-124">Not supported.</span></span> |
| <span data-ttu-id="066fe-125">Application</span><span class="sxs-lookup"><span data-stu-id="066fe-125">Application</span></span> | <span data-ttu-id="066fe-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="066fe-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="066fe-127">组</span><span class="sxs-lookup"><span data-stu-id="066fe-127">Groups</span></span>

|<span data-ttu-id="066fe-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="066fe-128">Permission type</span></span> | <span data-ttu-id="066fe-129">权限</span><span class="sxs-lookup"><span data-stu-id="066fe-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="066fe-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-130">Delegated (work or school account)</span></span> | <span data-ttu-id="066fe-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="066fe-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="066fe-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="066fe-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066fe-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="066fe-133">Not supported.</span></span> |
| <span data-ttu-id="066fe-134">Application</span><span class="sxs-lookup"><span data-stu-id="066fe-134">Application</span></span> | <span data-ttu-id="066fe-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="066fe-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="066fe-136">除了权限范围之外，此 API 要求请求程序至少具有一角色分配资源访问权限。</span><span class="sxs-lookup"><span data-stu-id="066fe-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="066fe-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="066fe-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="066fe-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="066fe-138">Optional query parameters</span></span>
<span data-ttu-id="066fe-139">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="066fe-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="066fe-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="066fe-140">Request headers</span></span>
| <span data-ttu-id="066fe-141">名称</span><span class="sxs-lookup"><span data-stu-id="066fe-141">Name</span></span>      |<span data-ttu-id="066fe-142">说明</span><span class="sxs-lookup"><span data-stu-id="066fe-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="066fe-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="066fe-143">Authorization</span></span>  | <span data-ttu-id="066fe-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="066fe-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="066fe-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="066fe-145">Request body</span></span>
<span data-ttu-id="066fe-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="066fe-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="066fe-147">响应</span><span class="sxs-lookup"><span data-stu-id="066fe-147">Response</span></span>
<span data-ttu-id="066fe-148">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 governanceRoleDefinition](../resources/governanceroledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="066fe-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="066fe-149">示例</span><span class="sxs-lookup"><span data-stu-id="066fe-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="066fe-150">此示例演示如何获取订阅 Wingtip Toys - Prod 的所有角色定义。</span><span class="sxs-lookup"><span data-stu-id="066fe-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="066fe-151">请求</span><span class="sxs-lookup"><span data-stu-id="066fe-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="066fe-152">响应</span><span class="sxs-lookup"><span data-stu-id="066fe-152">Response</span></span>
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



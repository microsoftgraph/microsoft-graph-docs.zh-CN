---
title: 获取 governanceRoleDefinition
description: 检索 governanceRoleDefinition 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1e9a2f52ea264f7bbcf3353e68deb9f51378efd1
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634975"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="2d760-103">获取 governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2d760-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="2d760-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d760-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d760-105">检索 [governanceRoleDefinition](../resources/governanceroledefinition.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d760-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d760-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d760-106">Permissions</span></span>
<span data-ttu-id="2d760-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="2d760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="2d760-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="2d760-109">Azure resources</span></span>

| <span data-ttu-id="2d760-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d760-110">Permission type</span></span> | <span data-ttu-id="2d760-111">权限</span><span class="sxs-lookup"><span data-stu-id="2d760-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2d760-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d760-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2d760-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="2d760-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d760-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d760-115">Not supported.</span></span> |
| <span data-ttu-id="2d760-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d760-116">Application</span></span> | <span data-ttu-id="2d760-117">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="2d760-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="2d760-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="2d760-118">Azure AD</span></span>

| <span data-ttu-id="2d760-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d760-119">Permission type</span></span> | <span data-ttu-id="2d760-120">权限</span><span class="sxs-lookup"><span data-stu-id="2d760-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2d760-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2d760-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2d760-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="2d760-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d760-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d760-124">Not supported.</span></span> |
| <span data-ttu-id="2d760-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d760-125">Application</span></span> | <span data-ttu-id="2d760-126">PrivilegedAccess。 AzureAD</span><span class="sxs-lookup"><span data-stu-id="2d760-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="2d760-127">组</span><span class="sxs-lookup"><span data-stu-id="2d760-127">Groups</span></span>

|<span data-ttu-id="2d760-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d760-128">Permission type</span></span> | <span data-ttu-id="2d760-129">权限</span><span class="sxs-lookup"><span data-stu-id="2d760-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="2d760-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-130">Delegated (work or school account)</span></span> | <span data-ttu-id="2d760-131">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="2d760-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="2d760-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d760-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d760-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d760-133">Not supported.</span></span> |
| <span data-ttu-id="2d760-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d760-134">Application</span></span> | <span data-ttu-id="2d760-135">PrivilegedAccess。 AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="2d760-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="2d760-136">除了权限范围之外，此 API 还要求请求者在资源上至少具有一个角色分配， [governanceRoleDefinition](../resources/governanceroledefinition.md) 属于该资源。</span><span class="sxs-lookup"><span data-stu-id="2d760-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="2d760-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d760-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d760-138">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="2d760-138">Optional query parameters</span></span>
<span data-ttu-id="2d760-139">此方法 **不** 支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2d760-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d760-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d760-140">Request headers</span></span>
| <span data-ttu-id="2d760-141">名称</span><span class="sxs-lookup"><span data-stu-id="2d760-141">Name</span></span>      |<span data-ttu-id="2d760-142">说明</span><span class="sxs-lookup"><span data-stu-id="2d760-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d760-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d760-143">Authorization</span></span>  | <span data-ttu-id="2d760-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2d760-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="2d760-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d760-145">Request body</span></span>
<span data-ttu-id="2d760-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d760-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2d760-147">响应</span><span class="sxs-lookup"><span data-stu-id="2d760-147">Response</span></span>
<span data-ttu-id="2d760-148">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [governanceRoleDefinition](../resources/governanceroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d760-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d760-149">示例</span><span class="sxs-lookup"><span data-stu-id="2d760-149">Example</span></span>
<span data-ttu-id="2d760-150">本示例演示如何在订阅 Wingtip 玩具-生产中获取角色定义 DNS 区域参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2d760-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="2d760-151">请求</span><span class="sxs-lookup"><span data-stu-id="2d760-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="2d760-152">响应</span><span class="sxs-lookup"><span data-stu-id="2d760-152">Response</span></span>
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



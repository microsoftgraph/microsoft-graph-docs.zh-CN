---
title: governanceResource 资源类型
description: 表示由 PIM 管理员的 Privileged Identity Management (管理) 。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL数据库等）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e0cf42593a35103996217d1ce18bd9938b48a185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443110"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="25469-104">governanceResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="25469-104">governanceResource resource type</span></span>

<span data-ttu-id="25469-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25469-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25469-106">表示由 PIM 管理员的 Privileged Identity Management (管理) 。</span><span class="sxs-lookup"><span data-stu-id="25469-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="25469-107">对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL数据库等）。</span><span class="sxs-lookup"><span data-stu-id="25469-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="25469-108">Methods</span><span class="sxs-lookup"><span data-stu-id="25469-108">Methods</span></span>

| <span data-ttu-id="25469-109">方法</span><span class="sxs-lookup"><span data-stu-id="25469-109">Method</span></span>          | <span data-ttu-id="25469-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="25469-110">Return Type</span></span> |<span data-ttu-id="25469-111">Description</span><span class="sxs-lookup"><span data-stu-id="25469-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25469-112">List</span><span class="sxs-lookup"><span data-stu-id="25469-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="25469-113">[governanceResource](../resources/governanceresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25469-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="25469-114">列出请求者有权访问的资源集合。</span><span class="sxs-lookup"><span data-stu-id="25469-114">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="25469-115">获取</span><span class="sxs-lookup"><span data-stu-id="25469-115">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="25469-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="25469-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="25469-117">读取由 id 指定的资源实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25469-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="25469-118">报名</span><span class="sxs-lookup"><span data-stu-id="25469-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="25469-119">将非托管 Azure 订阅或管理组注册到 PIM 服务。</span><span class="sxs-lookup"><span data-stu-id="25469-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="25469-120">现在 `POST` `PUT` ， `PATCH` `DELETE` 实体集上不支持否 `roleDefinitions` ，。</span><span class="sxs-lookup"><span data-stu-id="25469-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="25469-121">属性</span><span class="sxs-lookup"><span data-stu-id="25469-121">Properties</span></span>
| <span data-ttu-id="25469-122">属性</span><span class="sxs-lookup"><span data-stu-id="25469-122">Property</span></span>          |<span data-ttu-id="25469-123">类型</span><span class="sxs-lookup"><span data-stu-id="25469-123">Type</span></span>         |<span data-ttu-id="25469-124">说明</span><span class="sxs-lookup"><span data-stu-id="25469-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="25469-125">id</span><span class="sxs-lookup"><span data-stu-id="25469-125">id</span></span>                 |<span data-ttu-id="25469-126">String</span><span class="sxs-lookup"><span data-stu-id="25469-126">String</span></span>     |<span data-ttu-id="25469-127">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="25469-127">The id of the resource.</span></span> <span data-ttu-id="25469-128">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="25469-128">It is in GUID format.</span></span>|
|<span data-ttu-id="25469-129">externalId</span><span class="sxs-lookup"><span data-stu-id="25469-129">externalId</span></span>           |<span data-ttu-id="25469-130">String</span><span class="sxs-lookup"><span data-stu-id="25469-130">String</span></span>   |<span data-ttu-id="25469-131">资源的外部 ID，表示其外部系统中的原始 ID。</span><span class="sxs-lookup"><span data-stu-id="25469-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="25469-132">例如，订阅资源的外部 ID 可以是"/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。</span><span class="sxs-lookup"><span data-stu-id="25469-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="25469-133">type</span><span class="sxs-lookup"><span data-stu-id="25469-133">type</span></span>               |<span data-ttu-id="25469-134">String</span><span class="sxs-lookup"><span data-stu-id="25469-134">String</span></span>     |<span data-ttu-id="25469-135">必需。</span><span class="sxs-lookup"><span data-stu-id="25469-135">Required.</span></span> <span data-ttu-id="25469-136">资源类型。</span><span class="sxs-lookup"><span data-stu-id="25469-136">Resource type.</span></span> <span data-ttu-id="25469-137">例如，对于 Azure 资源，类型可以是"Subscription"、"ResourceGroup"、"Microsoft.Sql/server"等。</span><span class="sxs-lookup"><span data-stu-id="25469-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="25469-138">displayName</span><span class="sxs-lookup"><span data-stu-id="25469-138">displayName</span></span>        |<span data-ttu-id="25469-139">String</span><span class="sxs-lookup"><span data-stu-id="25469-139">String</span></span>     |<span data-ttu-id="25469-140">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="25469-140">The display name of the resource.</span></span>|
|<span data-ttu-id="25469-141">status</span><span class="sxs-lookup"><span data-stu-id="25469-141">status</span></span>             |<span data-ttu-id="25469-142">String</span><span class="sxs-lookup"><span data-stu-id="25469-142">String</span></span>     |<span data-ttu-id="25469-143">给定资源的状态。</span><span class="sxs-lookup"><span data-stu-id="25469-143">The status of a given resource.</span></span> <span data-ttu-id="25469-144">例如，它可以表示资源是否已锁定 (值 `Active` / `Locked` ：) 。</span><span class="sxs-lookup"><span data-stu-id="25469-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="25469-145">注意：将来可能会扩展此属性以支持更多方案。</span><span class="sxs-lookup"><span data-stu-id="25469-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="25469-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="25469-146">registeredDateTime</span></span>|<span data-ttu-id="25469-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25469-147">DateTimeOffset</span></span>      |<span data-ttu-id="25469-148">表示在 PIM 中注册资源的日期时间。</span><span class="sxs-lookup"><span data-stu-id="25469-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="25469-149">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="25469-149">registeredRoot</span></span>|<span data-ttu-id="25469-150">String</span><span class="sxs-lookup"><span data-stu-id="25469-150">String</span></span>      |<span data-ttu-id="25469-151">在 PIM 中注册的资源根作用域的 externalId。</span><span class="sxs-lookup"><span data-stu-id="25469-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="25469-152">根范围可以是父资源、父级资源或更高上级资源。</span><span class="sxs-lookup"><span data-stu-id="25469-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="25469-153">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="25469-153">roleAssignmentCount</span></span>|<span data-ttu-id="25469-154">Int32</span><span class="sxs-lookup"><span data-stu-id="25469-154">Int32</span></span>      |<span data-ttu-id="25469-155">可选。</span><span class="sxs-lookup"><span data-stu-id="25469-155">Optional.</span></span> <span data-ttu-id="25469-156">给定资源的角色分配数。</span><span class="sxs-lookup"><span data-stu-id="25469-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="25469-157">若要获取属性，请在查询中 `$select=roleAssignmentCount` 特地使用。</span><span class="sxs-lookup"><span data-stu-id="25469-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="25469-158">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="25469-158">roleDefinitionCount</span></span>|<span data-ttu-id="25469-159">Int32</span><span class="sxs-lookup"><span data-stu-id="25469-159">Int32</span></span>      |<span data-ttu-id="25469-160">可选。</span><span class="sxs-lookup"><span data-stu-id="25469-160">Optional.</span></span> <span data-ttu-id="25469-161">给定资源的角色定义数。</span><span class="sxs-lookup"><span data-stu-id="25469-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="25469-162">若要获取属性，请在查询中 `$select=roleDefinitionCount` 特地使用。</span><span class="sxs-lookup"><span data-stu-id="25469-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="25469-163">permissions</span><span class="sxs-lookup"><span data-stu-id="25469-163">permissions</span></span>|[<span data-ttu-id="25469-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="25469-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="25469-165">可选。</span><span class="sxs-lookup"><span data-stu-id="25469-165">Optional.</span></span> <span data-ttu-id="25469-166">它表示请求者对资源的访问权限的状态。若要获取属性，请在查询中 `$select=permissions` 特地使用。</span><span class="sxs-lookup"><span data-stu-id="25469-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25469-167">关系</span><span class="sxs-lookup"><span data-stu-id="25469-167">Relationships</span></span>
| <span data-ttu-id="25469-168">关系</span><span class="sxs-lookup"><span data-stu-id="25469-168">Relationship</span></span>   | <span data-ttu-id="25469-169">类型</span><span class="sxs-lookup"><span data-stu-id="25469-169">Type</span></span>                                         |<span data-ttu-id="25469-170">说明</span><span class="sxs-lookup"><span data-stu-id="25469-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="25469-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="25469-171">roleAssignments</span></span> |<span data-ttu-id="25469-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25469-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="25469-173">资源的角色分配集合。</span><span class="sxs-lookup"><span data-stu-id="25469-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="25469-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="25469-174">roleDefinitions</span></span> |<span data-ttu-id="25469-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25469-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="25469-176">资源的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="25469-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="25469-177">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="25469-177">roleAssignmentRequests</span></span> |<span data-ttu-id="25469-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25469-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="25469-179">资源角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="25469-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="25469-180">roleSettings</span><span class="sxs-lookup"><span data-stu-id="25469-180">roleSettings</span></span> |<span data-ttu-id="25469-181">[governanceRoleSetting](../resources/governancerolesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25469-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="25469-182">资源的角色设置集合。</span><span class="sxs-lookup"><span data-stu-id="25469-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="25469-183">父级</span><span class="sxs-lookup"><span data-stu-id="25469-183">parent</span></span>          |[<span data-ttu-id="25469-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="25469-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="25469-185">只读。</span><span class="sxs-lookup"><span data-stu-id="25469-185">Read-only.</span></span> <span data-ttu-id="25469-186">父资源。</span><span class="sxs-lookup"><span data-stu-id="25469-186">The parent resource.</span></span> <span data-ttu-id="25469-187">对于 `pimforazurerbac` 方案，它可以表示资源所属的订阅。</span><span class="sxs-lookup"><span data-stu-id="25469-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25469-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25469-188">JSON representation</span></span>

<span data-ttu-id="25469-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25469-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



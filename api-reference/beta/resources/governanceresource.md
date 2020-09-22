---
title: governanceResource 资源类型
description: 表示可由特权身份管理 (PIM) 管理的资源。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL 数据库等）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 4cfc4232fccf5c68649223746fdad853883166b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058384"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="ab073-104">governanceResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab073-104">governanceResource resource type</span></span>

<span data-ttu-id="ab073-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab073-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab073-106">表示可由特权身份管理 (PIM) 管理的资源。</span><span class="sxs-lookup"><span data-stu-id="ab073-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="ab073-107">对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL 数据库等）。</span><span class="sxs-lookup"><span data-stu-id="ab073-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="ab073-108">方法</span><span class="sxs-lookup"><span data-stu-id="ab073-108">Methods</span></span>

| <span data-ttu-id="ab073-109">方法</span><span class="sxs-lookup"><span data-stu-id="ab073-109">Method</span></span>          | <span data-ttu-id="ab073-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab073-110">Return Type</span></span> |<span data-ttu-id="ab073-111">Description</span><span class="sxs-lookup"><span data-stu-id="ab073-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab073-112">List</span><span class="sxs-lookup"><span data-stu-id="ab073-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="ab073-113">[governanceResource](../resources/governanceresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab073-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="ab073-114">列出请求者有权访问的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="ab073-114">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="ab073-115">Get</span><span class="sxs-lookup"><span data-stu-id="ab073-115">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="ab073-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="ab073-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="ab073-117">读取由 id 指定的资源实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab073-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="ab073-118">报名</span><span class="sxs-lookup"><span data-stu-id="ab073-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="ab073-119">将非托管 Azure 订阅或管理组注册到 PIM 服务。</span><span class="sxs-lookup"><span data-stu-id="ab073-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="ab073-120">`POST`目前， `PUT` `PATCH` `DELETE` entity set 上不支持，， `roleDefinitions` 。</span><span class="sxs-lookup"><span data-stu-id="ab073-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="ab073-121">属性</span><span class="sxs-lookup"><span data-stu-id="ab073-121">Properties</span></span>
| <span data-ttu-id="ab073-122">属性</span><span class="sxs-lookup"><span data-stu-id="ab073-122">Property</span></span>          |<span data-ttu-id="ab073-123">类型</span><span class="sxs-lookup"><span data-stu-id="ab073-123">Type</span></span>         |<span data-ttu-id="ab073-124">说明</span><span class="sxs-lookup"><span data-stu-id="ab073-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="ab073-125">id</span><span class="sxs-lookup"><span data-stu-id="ab073-125">id</span></span>                 |<span data-ttu-id="ab073-126">String</span><span class="sxs-lookup"><span data-stu-id="ab073-126">String</span></span>     |<span data-ttu-id="ab073-127">资源的 id。</span><span class="sxs-lookup"><span data-stu-id="ab073-127">The id of the resource.</span></span> <span data-ttu-id="ab073-128">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="ab073-128">It is in GUID format.</span></span>|
|<span data-ttu-id="ab073-129">externalId</span><span class="sxs-lookup"><span data-stu-id="ab073-129">externalId</span></span>           |<span data-ttu-id="ab073-130">String</span><span class="sxs-lookup"><span data-stu-id="ab073-130">String</span></span>   |<span data-ttu-id="ab073-131">资源的外部 id，表示其在外部系统中的原始 id。</span><span class="sxs-lookup"><span data-stu-id="ab073-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="ab073-132">例如，订阅资源的外部 id 可以是 "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。</span><span class="sxs-lookup"><span data-stu-id="ab073-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="ab073-133">type</span><span class="sxs-lookup"><span data-stu-id="ab073-133">type</span></span>               |<span data-ttu-id="ab073-134">String</span><span class="sxs-lookup"><span data-stu-id="ab073-134">String</span></span>     |<span data-ttu-id="ab073-135">必需。</span><span class="sxs-lookup"><span data-stu-id="ab073-135">Required.</span></span> <span data-ttu-id="ab073-136">资源类型。</span><span class="sxs-lookup"><span data-stu-id="ab073-136">Resource type.</span></span> <span data-ttu-id="ab073-137">例如，对于 Azure 资源，类型可以是 "订阅"、"ResourceGroup"、"Microsoft .Sql/服务器" 等。</span><span class="sxs-lookup"><span data-stu-id="ab073-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="ab073-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ab073-138">displayName</span></span>        |<span data-ttu-id="ab073-139">String</span><span class="sxs-lookup"><span data-stu-id="ab073-139">String</span></span>     |<span data-ttu-id="ab073-140">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ab073-140">The display name of the resource.</span></span>|
|<span data-ttu-id="ab073-141">状态</span><span class="sxs-lookup"><span data-stu-id="ab073-141">status</span></span>             |<span data-ttu-id="ab073-142">String</span><span class="sxs-lookup"><span data-stu-id="ab073-142">String</span></span>     |<span data-ttu-id="ab073-143">给定资源的状态。</span><span class="sxs-lookup"><span data-stu-id="ab073-143">The status of a given resource.</span></span> <span data-ttu-id="ab073-144">例如，它可以表示资源是否已锁定或不 (值： `Active` / `Locked`) 。</span><span class="sxs-lookup"><span data-stu-id="ab073-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="ab073-145">注意：将来可能会扩展此属性以支持更多方案。</span><span class="sxs-lookup"><span data-stu-id="ab073-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="ab073-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="ab073-146">registeredDateTime</span></span>|<span data-ttu-id="ab073-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab073-147">DateTimeOffset</span></span>      |<span data-ttu-id="ab073-148">表示在 PIM 中注册资源的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ab073-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="ab073-149">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="ab073-149">registeredRoot</span></span>|<span data-ttu-id="ab073-150">String</span><span class="sxs-lookup"><span data-stu-id="ab073-150">String</span></span>      |<span data-ttu-id="ab073-151">在 PIM 中注册的资源的根作用域的 externalId。</span><span class="sxs-lookup"><span data-stu-id="ab073-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="ab073-152">根作用域可以是父级、祖父或更高的上级资源。</span><span class="sxs-lookup"><span data-stu-id="ab073-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="ab073-153">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="ab073-153">roleAssignmentCount</span></span>|<span data-ttu-id="ab073-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ab073-154">Int32</span></span>      |<span data-ttu-id="ab073-155">可选。</span><span class="sxs-lookup"><span data-stu-id="ab073-155">Optional.</span></span> <span data-ttu-id="ab073-156">给定资源的角色分配数。</span><span class="sxs-lookup"><span data-stu-id="ab073-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="ab073-157">若要获取属性，请明确 `$select=roleAssignmentCount` 在查询中使用。</span><span class="sxs-lookup"><span data-stu-id="ab073-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="ab073-158">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="ab073-158">roleDefinitionCount</span></span>|<span data-ttu-id="ab073-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ab073-159">Int32</span></span>      |<span data-ttu-id="ab073-160">可选。</span><span class="sxs-lookup"><span data-stu-id="ab073-160">Optional.</span></span> <span data-ttu-id="ab073-161">给定资源的角色定义的数量。</span><span class="sxs-lookup"><span data-stu-id="ab073-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="ab073-162">若要获取属性，请明确 `$select=roleDefinitionCount` 在查询中使用。</span><span class="sxs-lookup"><span data-stu-id="ab073-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="ab073-163">permissions</span><span class="sxs-lookup"><span data-stu-id="ab073-163">permissions</span></span>|[<span data-ttu-id="ab073-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="ab073-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="ab073-165">可选。</span><span class="sxs-lookup"><span data-stu-id="ab073-165">Optional.</span></span> <span data-ttu-id="ab073-166">它表示请求者对资源的访问状态。若要获取属性，请明确 `$select=permissions` 在查询中使用。</span><span class="sxs-lookup"><span data-stu-id="ab073-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab073-167">关系</span><span class="sxs-lookup"><span data-stu-id="ab073-167">Relationships</span></span>
| <span data-ttu-id="ab073-168">关系</span><span class="sxs-lookup"><span data-stu-id="ab073-168">Relationship</span></span>   | <span data-ttu-id="ab073-169">类型</span><span class="sxs-lookup"><span data-stu-id="ab073-169">Type</span></span>                                         |<span data-ttu-id="ab073-170">说明</span><span class="sxs-lookup"><span data-stu-id="ab073-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="ab073-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="ab073-171">roleAssignments</span></span> |<span data-ttu-id="ab073-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab073-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="ab073-173">资源的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="ab073-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="ab073-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ab073-174">roleDefinitions</span></span> |<span data-ttu-id="ab073-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab073-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="ab073-176">资源的角色 defintions 集合。</span><span class="sxs-lookup"><span data-stu-id="ab073-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="ab073-177">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="ab073-177">roleAssignmentRequests</span></span> |<span data-ttu-id="ab073-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab073-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="ab073-179">资源的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="ab073-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="ab073-180">roleSettings</span><span class="sxs-lookup"><span data-stu-id="ab073-180">roleSettings</span></span> |<span data-ttu-id="ab073-181">[governanceRoleSetting](../resources/governancerolesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab073-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="ab073-182">资源的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="ab073-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="ab073-183">父级</span><span class="sxs-lookup"><span data-stu-id="ab073-183">parent</span></span>          |[<span data-ttu-id="ab073-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="ab073-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="ab073-185">只读。</span><span class="sxs-lookup"><span data-stu-id="ab073-185">Read-only.</span></span> <span data-ttu-id="ab073-186">父资源。</span><span class="sxs-lookup"><span data-stu-id="ab073-186">The parent resource.</span></span> <span data-ttu-id="ab073-187">对于 `pimforazurerbac` 方案，它可以表示资源所属的订阅。</span><span class="sxs-lookup"><span data-stu-id="ab073-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab073-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab073-188">JSON representation</span></span>

<span data-ttu-id="ab073-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab073-189">The following is a JSON representation of the resource.</span></span>

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



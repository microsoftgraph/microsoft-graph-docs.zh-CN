---
title: governanceResource 资源类型
description: 表示可由特权标识管理 (PIM) 管理的资源。 对于 Azure 资源, 它可以是订阅、资源组和资源 (如虚拟机、SQL 数据库等)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a0429de2cacc816eaf1a603a29a08897650da6e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971919"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="5996c-104">governanceResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="5996c-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5996c-105">表示可由特权标识管理 (PIM) 管理的资源。</span><span class="sxs-lookup"><span data-stu-id="5996c-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="5996c-106">对于 Azure 资源, 它可以是订阅、资源组和资源 (如虚拟机、SQL 数据库等)。</span><span class="sxs-lookup"><span data-stu-id="5996c-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="5996c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5996c-107">Methods</span></span>

| <span data-ttu-id="5996c-108">方法</span><span class="sxs-lookup"><span data-stu-id="5996c-108">Method</span></span>          | <span data-ttu-id="5996c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5996c-109">Return Type</span></span> |<span data-ttu-id="5996c-110">说明</span><span class="sxs-lookup"><span data-stu-id="5996c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5996c-111">List</span><span class="sxs-lookup"><span data-stu-id="5996c-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="5996c-112">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="5996c-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="5996c-113">列出请求者有权访问的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="5996c-113">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="5996c-114">获取</span><span class="sxs-lookup"><span data-stu-id="5996c-114">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="5996c-115">governanceResource</span><span class="sxs-lookup"><span data-stu-id="5996c-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="5996c-116">读取由 id 指定的资源实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5996c-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="5996c-117">报名</span><span class="sxs-lookup"><span data-stu-id="5996c-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="5996c-118">将非托管 Azure 订阅或管理组注册到 PIM 服务。</span><span class="sxs-lookup"><span data-stu-id="5996c-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="5996c-119">目前`POST`, `PUT`entity `PATCH`set `DELETE`上`roleDefinitions`不支持,,。</span><span class="sxs-lookup"><span data-stu-id="5996c-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="5996c-120">属性</span><span class="sxs-lookup"><span data-stu-id="5996c-120">Properties</span></span>
| <span data-ttu-id="5996c-121">属性</span><span class="sxs-lookup"><span data-stu-id="5996c-121">Property</span></span>          |<span data-ttu-id="5996c-122">类型</span><span class="sxs-lookup"><span data-stu-id="5996c-122">Type</span></span>         |<span data-ttu-id="5996c-123">说明</span><span class="sxs-lookup"><span data-stu-id="5996c-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="5996c-124">id</span><span class="sxs-lookup"><span data-stu-id="5996c-124">id</span></span>                 |<span data-ttu-id="5996c-125">String</span><span class="sxs-lookup"><span data-stu-id="5996c-125">String</span></span>     |<span data-ttu-id="5996c-126">资源的 id。</span><span class="sxs-lookup"><span data-stu-id="5996c-126">The id of the resource.</span></span> <span data-ttu-id="5996c-127">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="5996c-127">It is in GUID format.</span></span>|
|<span data-ttu-id="5996c-128">externalId</span><span class="sxs-lookup"><span data-stu-id="5996c-128">externalId</span></span>           |<span data-ttu-id="5996c-129">String</span><span class="sxs-lookup"><span data-stu-id="5996c-129">String</span></span>   |<span data-ttu-id="5996c-130">资源的外部 id, 表示其在外部系统中的原始 id。</span><span class="sxs-lookup"><span data-stu-id="5996c-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="5996c-131">例如, 订阅资源的外部 id 可以是 "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。</span><span class="sxs-lookup"><span data-stu-id="5996c-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="5996c-132">type</span><span class="sxs-lookup"><span data-stu-id="5996c-132">type</span></span>               |<span data-ttu-id="5996c-133">String</span><span class="sxs-lookup"><span data-stu-id="5996c-133">String</span></span>     |<span data-ttu-id="5996c-134">必需。</span><span class="sxs-lookup"><span data-stu-id="5996c-134">Required.</span></span> <span data-ttu-id="5996c-135">资源类型。</span><span class="sxs-lookup"><span data-stu-id="5996c-135">Resource type.</span></span> <span data-ttu-id="5996c-136">例如, 对于 Azure 资源, 类型可以是 "订阅"、"ResourceGroup"、"Microsoft .Sql/服务器" 等。</span><span class="sxs-lookup"><span data-stu-id="5996c-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="5996c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5996c-137">displayName</span></span>        |<span data-ttu-id="5996c-138">String</span><span class="sxs-lookup"><span data-stu-id="5996c-138">String</span></span>     |<span data-ttu-id="5996c-139">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5996c-139">The display name of the resource.</span></span>|
|<span data-ttu-id="5996c-140">status</span><span class="sxs-lookup"><span data-stu-id="5996c-140">status</span></span>             |<span data-ttu-id="5996c-141">String</span><span class="sxs-lookup"><span data-stu-id="5996c-141">String</span></span>     |<span data-ttu-id="5996c-142">给定资源的状态。</span><span class="sxs-lookup"><span data-stu-id="5996c-142">The status of a given resource.</span></span> <span data-ttu-id="5996c-143">例如, 它可以表示资源是否已锁定 (values: `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="5996c-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="5996c-144">注意: 将来可能会扩展此属性以支持更多方案。</span><span class="sxs-lookup"><span data-stu-id="5996c-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="5996c-145">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="5996c-145">registeredDateTime</span></span>|<span data-ttu-id="5996c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5996c-146">DateTimeOffset</span></span>      |<span data-ttu-id="5996c-147">表示在 PIM 中注册资源的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5996c-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="5996c-148">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="5996c-148">registeredRoot</span></span>|<span data-ttu-id="5996c-149">String</span><span class="sxs-lookup"><span data-stu-id="5996c-149">String</span></span>      |<span data-ttu-id="5996c-150">在 PIM 中注册的资源的根作用域的 externalId。</span><span class="sxs-lookup"><span data-stu-id="5996c-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="5996c-151">根作用域可以是父级、祖父或更高的上级资源。</span><span class="sxs-lookup"><span data-stu-id="5996c-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="5996c-152">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="5996c-152">roleAssignmentCount</span></span>|<span data-ttu-id="5996c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5996c-153">Int32</span></span>      |<span data-ttu-id="5996c-154">可选。</span><span class="sxs-lookup"><span data-stu-id="5996c-154">Optional.</span></span> <span data-ttu-id="5996c-155">给定资源的角色分配数。</span><span class="sxs-lookup"><span data-stu-id="5996c-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="5996c-156">若要获取属性, 请明确在`$select=roleAssignmentCount`查询中使用。</span><span class="sxs-lookup"><span data-stu-id="5996c-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="5996c-157">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="5996c-157">roleDefinitionCount</span></span>|<span data-ttu-id="5996c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5996c-158">Int32</span></span>      |<span data-ttu-id="5996c-159">可选。</span><span class="sxs-lookup"><span data-stu-id="5996c-159">Optional.</span></span> <span data-ttu-id="5996c-160">给定资源的角色定义的数量。</span><span class="sxs-lookup"><span data-stu-id="5996c-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="5996c-161">若要获取属性, 请明确在`$select=roleDefinitionCount`查询中使用。</span><span class="sxs-lookup"><span data-stu-id="5996c-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="5996c-162">permissions</span><span class="sxs-lookup"><span data-stu-id="5996c-162">permissions</span></span>|[<span data-ttu-id="5996c-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="5996c-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="5996c-164">可选。</span><span class="sxs-lookup"><span data-stu-id="5996c-164">Optional.</span></span> <span data-ttu-id="5996c-165">它表示请求者对资源的访问状态。若要获取属性, 请明确在`$select=permissions`查询中使用。</span><span class="sxs-lookup"><span data-stu-id="5996c-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5996c-166">关系</span><span class="sxs-lookup"><span data-stu-id="5996c-166">Relationships</span></span>
| <span data-ttu-id="5996c-167">关系</span><span class="sxs-lookup"><span data-stu-id="5996c-167">Relationship</span></span>   | <span data-ttu-id="5996c-168">类型</span><span class="sxs-lookup"><span data-stu-id="5996c-168">Type</span></span>                                         |<span data-ttu-id="5996c-169">说明</span><span class="sxs-lookup"><span data-stu-id="5996c-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="5996c-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="5996c-170">roleAssignments</span></span> |<span data-ttu-id="5996c-171">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5996c-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="5996c-172">资源的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="5996c-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="5996c-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="5996c-173">roleDefinitions</span></span> |<span data-ttu-id="5996c-174">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="5996c-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="5996c-175">资源的角色 defintions 集合。</span><span class="sxs-lookup"><span data-stu-id="5996c-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="5996c-176">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="5996c-176">roleAssignmentRequests</span></span> |<span data-ttu-id="5996c-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="5996c-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="5996c-178">资源的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="5996c-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="5996c-179">roleSettings</span><span class="sxs-lookup"><span data-stu-id="5996c-179">roleSettings</span></span> |<span data-ttu-id="5996c-180">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5996c-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="5996c-181">资源的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="5996c-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="5996c-182">母语</span><span class="sxs-lookup"><span data-stu-id="5996c-182">parent</span></span>          |[<span data-ttu-id="5996c-183">governanceResource</span><span class="sxs-lookup"><span data-stu-id="5996c-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="5996c-184">只读。</span><span class="sxs-lookup"><span data-stu-id="5996c-184">Read-only.</span></span> <span data-ttu-id="5996c-185">父资源。</span><span class="sxs-lookup"><span data-stu-id="5996c-185">The parent resource.</span></span> <span data-ttu-id="5996c-186">对于`pimforazurerbac`方案, 它可以表示资源所属的订阅。</span><span class="sxs-lookup"><span data-stu-id="5996c-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5996c-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5996c-187">JSON representation</span></span>

<span data-ttu-id="5996c-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5996c-188">The following is a JSON representation of the resource.</span></span>

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

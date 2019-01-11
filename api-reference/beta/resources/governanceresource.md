---
title: governanceResource 资源类型
description: 表示无法管理特权标识管理 (PIM) 的资源。 有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。
localization_priority: Normal
ms.openlocfilehash: 263996049753256fd39906dba61138c3ab0f0248
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869389"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="0206d-104">governanceResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="0206d-104">governanceResource resource type</span></span>

> <span data-ttu-id="0206d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0206d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0206d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0206d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0206d-107">表示无法管理特权标识管理 (PIM) 的资源。</span><span class="sxs-lookup"><span data-stu-id="0206d-107">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="0206d-108">有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。</span><span class="sxs-lookup"><span data-stu-id="0206d-108">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="0206d-109">方法</span><span class="sxs-lookup"><span data-stu-id="0206d-109">Methods</span></span>

| <span data-ttu-id="0206d-110">方法</span><span class="sxs-lookup"><span data-stu-id="0206d-110">Method</span></span>          | <span data-ttu-id="0206d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0206d-111">Return Type</span></span> |<span data-ttu-id="0206d-112">说明</span><span class="sxs-lookup"><span data-stu-id="0206d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0206d-113">List</span><span class="sxs-lookup"><span data-stu-id="0206d-113">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="0206d-114">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="0206d-114">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="0206d-115">列出请求者有权访问的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="0206d-115">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="0206d-116">Get</span><span class="sxs-lookup"><span data-stu-id="0206d-116">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="0206d-117">governanceResource</span><span class="sxs-lookup"><span data-stu-id="0206d-117">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="0206d-118">读取属性并由 id 指定的资源实体的关系。</span><span class="sxs-lookup"><span data-stu-id="0206d-118">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="0206d-119">注册</span><span class="sxs-lookup"><span data-stu-id="0206d-119">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="0206d-120">注册 PIM 服务非托管 Azure 订阅或管理组。</span><span class="sxs-lookup"><span data-stu-id="0206d-120">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="0206d-121">不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。</span><span class="sxs-lookup"><span data-stu-id="0206d-121">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="0206d-122">属性</span><span class="sxs-lookup"><span data-stu-id="0206d-122">Properties</span></span>
| <span data-ttu-id="0206d-123">属性</span><span class="sxs-lookup"><span data-stu-id="0206d-123">Property</span></span>          |<span data-ttu-id="0206d-124">类型</span><span class="sxs-lookup"><span data-stu-id="0206d-124">Type</span></span>         |<span data-ttu-id="0206d-125">说明</span><span class="sxs-lookup"><span data-stu-id="0206d-125">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="0206d-126">id</span><span class="sxs-lookup"><span data-stu-id="0206d-126">id</span></span>                 |<span data-ttu-id="0206d-127">字符串</span><span class="sxs-lookup"><span data-stu-id="0206d-127">String</span></span>     |<span data-ttu-id="0206d-128">资源的 id。</span><span class="sxs-lookup"><span data-stu-id="0206d-128">The id of the resource.</span></span> <span data-ttu-id="0206d-129">处于 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="0206d-129">It is in GUID format.</span></span>|
|<span data-ttu-id="0206d-130">externalId</span><span class="sxs-lookup"><span data-stu-id="0206d-130">externalId</span></span>           |<span data-ttu-id="0206d-131">String</span><span class="sxs-lookup"><span data-stu-id="0206d-131">String</span></span>   |<span data-ttu-id="0206d-132">外部资源，表示其原始 id 外部系统中的 id。</span><span class="sxs-lookup"><span data-stu-id="0206d-132">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="0206d-133">例如，订阅资源的外部 id 可以是"/ 订阅/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。</span><span class="sxs-lookup"><span data-stu-id="0206d-133">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="0206d-134">type</span><span class="sxs-lookup"><span data-stu-id="0206d-134">type</span></span>               |<span data-ttu-id="0206d-135">字符串</span><span class="sxs-lookup"><span data-stu-id="0206d-135">String</span></span>     |<span data-ttu-id="0206d-136">必需。</span><span class="sxs-lookup"><span data-stu-id="0206d-136">Required.</span></span> <span data-ttu-id="0206d-137">资源类型。</span><span class="sxs-lookup"><span data-stu-id="0206d-137">Resource type.</span></span> <span data-ttu-id="0206d-138">例如，对于 Azure 资源，键入无法为"订阅"、"ResourceGroup"、"Microsoft.Sql/server"等。</span><span class="sxs-lookup"><span data-stu-id="0206d-138">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="0206d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0206d-139">displayName</span></span>        |<span data-ttu-id="0206d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0206d-140">String</span></span>     |<span data-ttu-id="0206d-141">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0206d-141">The display name of the resource.</span></span>|
|<span data-ttu-id="0206d-142">status</span><span class="sxs-lookup"><span data-stu-id="0206d-142">status</span></span>             |<span data-ttu-id="0206d-143">字符串</span><span class="sxs-lookup"><span data-stu-id="0206d-143">String</span></span>     |<span data-ttu-id="0206d-144">给定资源的状态。</span><span class="sxs-lookup"><span data-stu-id="0206d-144">The status of a given resource.</span></span> <span data-ttu-id="0206d-145">例如，它可能表示是否资源被锁定或未 (值： `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="0206d-145">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="0206d-146">注意： 该属性可能进行扩展，以便将来以支持更多方案。</span><span class="sxs-lookup"><span data-stu-id="0206d-146">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="0206d-147">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="0206d-147">registeredDateTime</span></span>|<span data-ttu-id="0206d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0206d-148">DateTimeOffset</span></span>      |<span data-ttu-id="0206d-149">代表资源中 PIM 的注册时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="0206d-149">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="0206d-150">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="0206d-150">registeredRoot</span></span>|<span data-ttu-id="0206d-151">字符串</span><span class="sxs-lookup"><span data-stu-id="0206d-151">String</span></span>      |<span data-ttu-id="0206d-152">PIM 中注册的资源的根范围 externalId。</span><span class="sxs-lookup"><span data-stu-id="0206d-152">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="0206d-153">根范围可以是父、 祖父或更高版本上级资源。</span><span class="sxs-lookup"><span data-stu-id="0206d-153">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="0206d-154">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="0206d-154">roleAssignmentCount</span></span>|<span data-ttu-id="0206d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0206d-155">Int32</span></span>      |<span data-ttu-id="0206d-156">可选。</span><span class="sxs-lookup"><span data-stu-id="0206d-156">Optional.</span></span> <span data-ttu-id="0206d-157">给定资源的角色分配的数目。</span><span class="sxs-lookup"><span data-stu-id="0206d-157">The number of role assignments for the given resource.</span></span> <span data-ttu-id="0206d-158">若要获取的属性，请是明确使用`$select=roleAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="0206d-158">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="0206d-159">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="0206d-159">roleDefinitionCount</span></span>|<span data-ttu-id="0206d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0206d-160">Int32</span></span>      |<span data-ttu-id="0206d-161">可选。</span><span class="sxs-lookup"><span data-stu-id="0206d-161">Optional.</span></span> <span data-ttu-id="0206d-162">给定资源的角色定义的数目。</span><span class="sxs-lookup"><span data-stu-id="0206d-162">The number of role definitions for the given resource.</span></span> <span data-ttu-id="0206d-163">若要获取的属性，请是明确使用`$select=roleDefinitionCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="0206d-163">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="0206d-164">permissions</span><span class="sxs-lookup"><span data-stu-id="0206d-164">permissions</span></span>|[<span data-ttu-id="0206d-165">governancePermission</span><span class="sxs-lookup"><span data-stu-id="0206d-165">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="0206d-166">可选。</span><span class="sxs-lookup"><span data-stu-id="0206d-166">Optional.</span></span> <span data-ttu-id="0206d-167">它表示对资源的请求者的访问状态。若要获取的属性，请是明确使用`$select=permissions`查询中。</span><span class="sxs-lookup"><span data-stu-id="0206d-167">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0206d-168">Relationships</span><span class="sxs-lookup"><span data-stu-id="0206d-168">Relationships</span></span>
| <span data-ttu-id="0206d-169">关系</span><span class="sxs-lookup"><span data-stu-id="0206d-169">Relationship</span></span>   | <span data-ttu-id="0206d-170">类型</span><span class="sxs-lookup"><span data-stu-id="0206d-170">Type</span></span>                                         |<span data-ttu-id="0206d-171">说明</span><span class="sxs-lookup"><span data-stu-id="0206d-171">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="0206d-172">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="0206d-172">roleAssignments</span></span> |<span data-ttu-id="0206d-173">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0206d-173">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="0206d-174">角色分配资源的集合。</span><span class="sxs-lookup"><span data-stu-id="0206d-174">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="0206d-175">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="0206d-175">roleDefinitions</span></span> |<span data-ttu-id="0206d-176">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="0206d-176">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="0206d-177">资源的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="0206d-177">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="0206d-178">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="0206d-178">roleAssignmentRequests</span></span> |<span data-ttu-id="0206d-179">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="0206d-179">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="0206d-180">角色分配请求资源的集合。</span><span class="sxs-lookup"><span data-stu-id="0206d-180">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="0206d-181">roleSettings</span><span class="sxs-lookup"><span data-stu-id="0206d-181">roleSettings</span></span> |<span data-ttu-id="0206d-182">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="0206d-182">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="0206d-183">资源角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="0206d-183">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="0206d-184">父</span><span class="sxs-lookup"><span data-stu-id="0206d-184">parent</span></span>          |[<span data-ttu-id="0206d-185">governanceResource</span><span class="sxs-lookup"><span data-stu-id="0206d-185">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="0206d-186">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="0206d-186">Read-only.</span></span> <span data-ttu-id="0206d-187">父资源。</span><span class="sxs-lookup"><span data-stu-id="0206d-187">The parent resource.</span></span> <span data-ttu-id="0206d-188">为`pimforazurerbac`方案中，它可以表示资源所属的订阅。</span><span class="sxs-lookup"><span data-stu-id="0206d-188">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0206d-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0206d-189">JSON representation</span></span>

<span data-ttu-id="0206d-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0206d-190">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: governanceResource 资源类型
description: 表示无法管理特权标识管理 (PIM) 的资源。 有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。
ms.openlocfilehash: 9e47f1295f9498796d51414a0a97acbe51fe1aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045753"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="9d059-104">governanceResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d059-104">governanceResource resource type</span></span>

> <span data-ttu-id="9d059-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d059-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d059-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d059-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d059-107">表示无法管理特权标识管理 (PIM) 的资源。</span><span class="sxs-lookup"><span data-stu-id="9d059-107">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="9d059-108">有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。</span><span class="sxs-lookup"><span data-stu-id="9d059-108">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="9d059-109">方法</span><span class="sxs-lookup"><span data-stu-id="9d059-109">Methods</span></span>

| <span data-ttu-id="9d059-110">方法</span><span class="sxs-lookup"><span data-stu-id="9d059-110">Method</span></span>          | <span data-ttu-id="9d059-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d059-111">Return Type</span></span> |<span data-ttu-id="9d059-112">说明</span><span class="sxs-lookup"><span data-stu-id="9d059-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d059-113">List</span><span class="sxs-lookup"><span data-stu-id="9d059-113">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="9d059-114">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d059-114">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="9d059-115">列出请求者有权访问的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9d059-115">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="9d059-116">Get</span><span class="sxs-lookup"><span data-stu-id="9d059-116">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="9d059-117">governanceResource</span><span class="sxs-lookup"><span data-stu-id="9d059-117">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="9d059-118">读取属性并由 id 指定的资源实体的关系。</span><span class="sxs-lookup"><span data-stu-id="9d059-118">Read properties and relationships of a resource entity specified by id.</span></span>|

<span data-ttu-id="9d059-119">不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。</span><span class="sxs-lookup"><span data-stu-id="9d059-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="9d059-120">属性</span><span class="sxs-lookup"><span data-stu-id="9d059-120">Properties</span></span>
| <span data-ttu-id="9d059-121">属性</span><span class="sxs-lookup"><span data-stu-id="9d059-121">Property</span></span>          |<span data-ttu-id="9d059-122">类型</span><span class="sxs-lookup"><span data-stu-id="9d059-122">Type</span></span>         |<span data-ttu-id="9d059-123">说明</span><span class="sxs-lookup"><span data-stu-id="9d059-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="9d059-124">id</span><span class="sxs-lookup"><span data-stu-id="9d059-124">id</span></span>                 |<span data-ttu-id="9d059-125">字符串</span><span class="sxs-lookup"><span data-stu-id="9d059-125">String</span></span>     |<span data-ttu-id="9d059-126">资源的 id。</span><span class="sxs-lookup"><span data-stu-id="9d059-126">The id of the resource.</span></span> <span data-ttu-id="9d059-127">处于 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="9d059-127">It is in GUID format.</span></span>|
|<span data-ttu-id="9d059-128">externalId</span><span class="sxs-lookup"><span data-stu-id="9d059-128">externalId</span></span>           |<span data-ttu-id="9d059-129">String</span><span class="sxs-lookup"><span data-stu-id="9d059-129">String</span></span>   |<span data-ttu-id="9d059-130">外部资源，表示其原始 id 外部数据库中的 id。</span><span class="sxs-lookup"><span data-stu-id="9d059-130">The external id of the resource, representing its original id in the external database.</span></span> <span data-ttu-id="9d059-131">例如，订阅资源的外部 id 可以是"/ 订阅/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。</span><span class="sxs-lookup"><span data-stu-id="9d059-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="9d059-132">type</span><span class="sxs-lookup"><span data-stu-id="9d059-132">type</span></span>               |<span data-ttu-id="9d059-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9d059-133">String</span></span>     |<span data-ttu-id="9d059-134">必需项。</span><span class="sxs-lookup"><span data-stu-id="9d059-134">Required.</span></span> <span data-ttu-id="9d059-135">资源类型。</span><span class="sxs-lookup"><span data-stu-id="9d059-135">Resource type.</span></span> <span data-ttu-id="9d059-136">例如，对于 Azure 资源，键入无法为"订阅"、"ResourceGroup"、"Microsoft.Sql/server"等。</span><span class="sxs-lookup"><span data-stu-id="9d059-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="9d059-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9d059-137">displayName</span></span>        |<span data-ttu-id="9d059-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9d059-138">String</span></span>     |<span data-ttu-id="9d059-139">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d059-139">The display name of the resource.</span></span>|
|<span data-ttu-id="9d059-140">状态</span><span class="sxs-lookup"><span data-stu-id="9d059-140">status</span></span>             |<span data-ttu-id="9d059-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9d059-141">String</span></span>     |<span data-ttu-id="9d059-142">给定资源的状态。</span><span class="sxs-lookup"><span data-stu-id="9d059-142">The status of a given resource.</span></span> <span data-ttu-id="9d059-143">例如，它可能表示是否资源被锁定或未 (值： `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="9d059-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="9d059-144">注意： 该属性可能进行扩展，以便将来以支持更多方案。</span><span class="sxs-lookup"><span data-stu-id="9d059-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="9d059-145">onboardDateTime</span><span class="sxs-lookup"><span data-stu-id="9d059-145">onboardDateTime</span></span>|<span data-ttu-id="9d059-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d059-146">DateTimeOffset</span></span>      |<span data-ttu-id="9d059-147">它表示由 PIM 管理的资源开始时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="9d059-147">It represents the date time when the resource starts to be managed by PIM.</span></span>|
|<span data-ttu-id="9d059-148">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="9d059-148">roleAssignmentCount</span></span>|<span data-ttu-id="9d059-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9d059-149">Int32</span></span>      |<span data-ttu-id="9d059-150">可选。</span><span class="sxs-lookup"><span data-stu-id="9d059-150">Optional.</span></span> <span data-ttu-id="9d059-151">给定资源的角色分配的数目。</span><span class="sxs-lookup"><span data-stu-id="9d059-151">The number of role assignments for the given resource.</span></span> <span data-ttu-id="9d059-152">若要获取的属性，请是明确使用`$select=roleAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="9d059-152">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="9d059-153">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="9d059-153">roleDefinitionCount</span></span>|<span data-ttu-id="9d059-154">Int32</span><span class="sxs-lookup"><span data-stu-id="9d059-154">Int32</span></span>      |<span data-ttu-id="9d059-155">可选。</span><span class="sxs-lookup"><span data-stu-id="9d059-155">Optional.</span></span> <span data-ttu-id="9d059-156">给定资源的角色定义的数目。</span><span class="sxs-lookup"><span data-stu-id="9d059-156">The number of role definitions for the given resource.</span></span> <span data-ttu-id="9d059-157">若要获取的属性，请是明确使用`$select=roleDefinitionCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="9d059-157">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="9d059-158">permissions</span><span class="sxs-lookup"><span data-stu-id="9d059-158">permissions</span></span>|[<span data-ttu-id="9d059-159">governancePermission</span><span class="sxs-lookup"><span data-stu-id="9d059-159">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="9d059-160">可选。</span><span class="sxs-lookup"><span data-stu-id="9d059-160">Optional.</span></span> <span data-ttu-id="9d059-161">它表示对资源的请求者的访问状态。若要获取的属性，请是明确使用`$select=permissions`查询中。</span><span class="sxs-lookup"><span data-stu-id="9d059-161">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d059-162">Relationships</span><span class="sxs-lookup"><span data-stu-id="9d059-162">Relationships</span></span>
| <span data-ttu-id="9d059-163">关系</span><span class="sxs-lookup"><span data-stu-id="9d059-163">Relationship</span></span>   | <span data-ttu-id="9d059-164">类型</span><span class="sxs-lookup"><span data-stu-id="9d059-164">Type</span></span>                                         |<span data-ttu-id="9d059-165">说明</span><span class="sxs-lookup"><span data-stu-id="9d059-165">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="9d059-166">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9d059-166">roleAssignments</span></span> |<span data-ttu-id="9d059-167">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d059-167">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="9d059-168">角色分配资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9d059-168">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="9d059-169">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="9d059-169">roleDefinitions</span></span> |<span data-ttu-id="9d059-170">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d059-170">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="9d059-171">资源的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="9d059-171">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="9d059-172">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9d059-172">roleAssignmentRequests</span></span> |<span data-ttu-id="9d059-173">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d059-173">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="9d059-174">角色分配请求资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9d059-174">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="9d059-175">roleSettings</span><span class="sxs-lookup"><span data-stu-id="9d059-175">roleSettings</span></span> |<span data-ttu-id="9d059-176">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d059-176">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="9d059-177">资源角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="9d059-177">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="9d059-178">父</span><span class="sxs-lookup"><span data-stu-id="9d059-178">parent</span></span>          |[<span data-ttu-id="9d059-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="9d059-179">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="9d059-180">只读。</span><span class="sxs-lookup"><span data-stu-id="9d059-180">Read-only.</span></span> <span data-ttu-id="9d059-181">父资源。</span><span class="sxs-lookup"><span data-stu-id="9d059-181">The parent resource.</span></span> <span data-ttu-id="9d059-182">为`pimforazurerbac`方案中，它可以表示资源所属的订阅。</span><span class="sxs-lookup"><span data-stu-id="9d059-182">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d059-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d059-183">JSON representation</span></span>

<span data-ttu-id="9d059-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d059-184">Here is a JSON representation of the resource.</span></span>

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
  "status": "String"
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
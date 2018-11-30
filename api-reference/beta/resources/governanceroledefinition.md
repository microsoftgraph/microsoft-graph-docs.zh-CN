---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043111"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="5d541-104">governanceRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d541-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="5d541-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d541-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d541-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d541-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="5d541-107">表示角色定义。</span><span class="sxs-lookup"><span data-stu-id="5d541-107">Represents the role definitions.</span></span> <span data-ttu-id="5d541-108">有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。</span><span class="sxs-lookup"><span data-stu-id="5d541-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="5d541-109">方法</span><span class="sxs-lookup"><span data-stu-id="5d541-109">Methods</span></span>

| <span data-ttu-id="5d541-110">方法</span><span class="sxs-lookup"><span data-stu-id="5d541-110">Method</span></span>          | <span data-ttu-id="5d541-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5d541-111">Return Type</span></span> |<span data-ttu-id="5d541-112">说明</span><span class="sxs-lookup"><span data-stu-id="5d541-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="5d541-113">List</span><span class="sxs-lookup"><span data-stu-id="5d541-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="5d541-114">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d541-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="5d541-115">列出对资源的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="5d541-115">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="5d541-116">Get</span><span class="sxs-lookup"><span data-stu-id="5d541-116">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="5d541-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5d541-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="5d541-118">读取的属性并由 id 指定的角色定义实体的关系。</span><span class="sxs-lookup"><span data-stu-id="5d541-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="5d541-119">不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。</span><span class="sxs-lookup"><span data-stu-id="5d541-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="5d541-120">属性</span><span class="sxs-lookup"><span data-stu-id="5d541-120">Properties</span></span>
| <span data-ttu-id="5d541-121">属性</span><span class="sxs-lookup"><span data-stu-id="5d541-121">Property</span></span>  | <span data-ttu-id="5d541-122">类型</span><span class="sxs-lookup"><span data-stu-id="5d541-122">Type</span></span>      |<span data-ttu-id="5d541-123">说明</span><span class="sxs-lookup"><span data-stu-id="5d541-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="5d541-124">id</span><span class="sxs-lookup"><span data-stu-id="5d541-124">id</span></span>         |<span data-ttu-id="5d541-125">字符串</span><span class="sxs-lookup"><span data-stu-id="5d541-125">String</span></span>     |<span data-ttu-id="5d541-126">角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="5d541-126">The id of the role definition.</span></span> |
|<span data-ttu-id="5d541-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="5d541-127">resourceId</span></span> |<span data-ttu-id="5d541-128">String</span><span class="sxs-lookup"><span data-stu-id="5d541-128">String</span></span>     |<span data-ttu-id="5d541-129">必需项。</span><span class="sxs-lookup"><span data-stu-id="5d541-129">Required.</span></span> <span data-ttu-id="5d541-130">与角色定义关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="5d541-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="5d541-131">externalId</span><span class="sxs-lookup"><span data-stu-id="5d541-131">externalId</span></span>   |<span data-ttu-id="5d541-132">String</span><span class="sxs-lookup"><span data-stu-id="5d541-132">String</span></span>     |<span data-ttu-id="5d541-133">外部角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="5d541-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="5d541-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5d541-134">displayName</span></span>|<span data-ttu-id="5d541-135">字符串</span><span class="sxs-lookup"><span data-stu-id="5d541-135">String</span></span>     |<span data-ttu-id="5d541-136">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5d541-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="5d541-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="5d541-137">subjectCount</span></span>|<span data-ttu-id="5d541-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5d541-138">Int32</span></span>     |<span data-ttu-id="5d541-139">可选。</span><span class="sxs-lookup"><span data-stu-id="5d541-139">Optional.</span></span> <span data-ttu-id="5d541-140">分配给角色的主题数。</span><span class="sxs-lookup"><span data-stu-id="5d541-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="5d541-141">它表示对资源的请求者的访问状态。</span><span class="sxs-lookup"><span data-stu-id="5d541-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="5d541-142">若要获取的属性，请是明确使用`$select=subjectCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="5d541-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="5d541-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="5d541-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="5d541-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5d541-144">Int32</span></span>|<span data-ttu-id="5d541-145">可选。</span><span class="sxs-lookup"><span data-stu-id="5d541-145">Optional.</span></span> <span data-ttu-id="5d541-146">合格的角色分配相关联的角色定义数。</span><span class="sxs-lookup"><span data-stu-id="5d541-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="5d541-147">若要获取的属性，请是明确使用`$select=eligibleAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="5d541-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="5d541-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="5d541-148">activeAssignmentCount</span></span>|<span data-ttu-id="5d541-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5d541-149">Int32</span></span>    |<span data-ttu-id="5d541-150">可选。</span><span class="sxs-lookup"><span data-stu-id="5d541-150">Optional.</span></span> <span data-ttu-id="5d541-151">活动的角色分配相关联的角色定义数。</span><span class="sxs-lookup"><span data-stu-id="5d541-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="5d541-152">若要获取的属性，请是明确使用`$select=activeAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="5d541-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5d541-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="5d541-153">Relationships</span></span>
| <span data-ttu-id="5d541-154">关系</span><span class="sxs-lookup"><span data-stu-id="5d541-154">Relationship</span></span> | <span data-ttu-id="5d541-155">类型</span><span class="sxs-lookup"><span data-stu-id="5d541-155">Type</span></span>   |<span data-ttu-id="5d541-156">说明</span><span class="sxs-lookup"><span data-stu-id="5d541-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d541-157">资源</span><span class="sxs-lookup"><span data-stu-id="5d541-157">resource</span></span>|[<span data-ttu-id="5d541-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="5d541-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="5d541-159">只读。</span><span class="sxs-lookup"><span data-stu-id="5d541-159">Read-only.</span></span> <span data-ttu-id="5d541-160">相关联的角色定义的资源。</span><span class="sxs-lookup"><span data-stu-id="5d541-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="5d541-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="5d541-161">roleSetting</span></span>|[<span data-ttu-id="5d541-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="5d541-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="5d541-163">角色定义关联的角色设置。</span><span class="sxs-lookup"><span data-stu-id="5d541-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d541-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d541-164">JSON representation</span></span>

<span data-ttu-id="5d541-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d541-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528639"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="7ab4c-104">governanceRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ab4c-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="7ab4c-105">表示角色定义。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-105">Represents the role definitions.</span></span> <span data-ttu-id="7ab4c-106">有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="7ab4c-107">方法</span><span class="sxs-lookup"><span data-stu-id="7ab4c-107">Methods</span></span>

| <span data-ttu-id="7ab4c-108">方法</span><span class="sxs-lookup"><span data-stu-id="7ab4c-108">Method</span></span>          | <span data-ttu-id="7ab4c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ab4c-109">Return Type</span></span> |<span data-ttu-id="7ab4c-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ab4c-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="7ab4c-111">List</span><span class="sxs-lookup"><span data-stu-id="7ab4c-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="7ab4c-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ab4c-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="7ab4c-113">列出对资源的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="7ab4c-114">Get</span><span class="sxs-lookup"><span data-stu-id="7ab4c-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="7ab4c-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab4c-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="7ab4c-116">读取的属性并由 id 指定的角色定义实体的关系。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="7ab4c-117">不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="7ab4c-118">属性</span><span class="sxs-lookup"><span data-stu-id="7ab4c-118">Properties</span></span>
| <span data-ttu-id="7ab4c-119">属性</span><span class="sxs-lookup"><span data-stu-id="7ab4c-119">Property</span></span>  | <span data-ttu-id="7ab4c-120">类型</span><span class="sxs-lookup"><span data-stu-id="7ab4c-120">Type</span></span>      |<span data-ttu-id="7ab4c-121">说明</span><span class="sxs-lookup"><span data-stu-id="7ab4c-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="7ab4c-122">id</span><span class="sxs-lookup"><span data-stu-id="7ab4c-122">id</span></span>         |<span data-ttu-id="7ab4c-123">字符串</span><span class="sxs-lookup"><span data-stu-id="7ab4c-123">String</span></span>     |<span data-ttu-id="7ab4c-124">角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-124">The id of the role definition.</span></span> |
|<span data-ttu-id="7ab4c-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="7ab4c-125">resourceId</span></span> |<span data-ttu-id="7ab4c-126">String</span><span class="sxs-lookup"><span data-stu-id="7ab4c-126">String</span></span>     |<span data-ttu-id="7ab4c-127">必需。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-127">Required.</span></span> <span data-ttu-id="7ab4c-128">与角色定义关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="7ab4c-129">externalId</span><span class="sxs-lookup"><span data-stu-id="7ab4c-129">externalId</span></span>   |<span data-ttu-id="7ab4c-130">String</span><span class="sxs-lookup"><span data-stu-id="7ab4c-130">String</span></span>     |<span data-ttu-id="7ab4c-131">外部角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="7ab4c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7ab4c-132">displayName</span></span>|<span data-ttu-id="7ab4c-133">String</span><span class="sxs-lookup"><span data-stu-id="7ab4c-133">String</span></span>     |<span data-ttu-id="7ab4c-134">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="7ab4c-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="7ab4c-135">subjectCount</span></span>|<span data-ttu-id="7ab4c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab4c-136">Int32</span></span>     |<span data-ttu-id="7ab4c-137">可选。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-137">Optional.</span></span> <span data-ttu-id="7ab4c-138">分配给角色的主题数。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="7ab4c-139">它表示对资源的请求者的访问状态。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="7ab4c-140">若要获取的属性，请是明确使用`$select=subjectCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="7ab4c-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="7ab4c-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="7ab4c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab4c-142">Int32</span></span>|<span data-ttu-id="7ab4c-143">可选。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-143">Optional.</span></span> <span data-ttu-id="7ab4c-144">合格的角色分配相关联的角色定义数。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="7ab4c-145">若要获取的属性，请是明确使用`$select=eligibleAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="7ab4c-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="7ab4c-146">activeAssignmentCount</span></span>|<span data-ttu-id="7ab4c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab4c-147">Int32</span></span>    |<span data-ttu-id="7ab4c-148">可选。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-148">Optional.</span></span> <span data-ttu-id="7ab4c-149">活动的角色分配相关联的角色定义数。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="7ab4c-150">若要获取的属性，请是明确使用`$select=activeAssignmentCount`查询中。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7ab4c-151">关系</span><span class="sxs-lookup"><span data-stu-id="7ab4c-151">Relationships</span></span>
| <span data-ttu-id="7ab4c-152">关系</span><span class="sxs-lookup"><span data-stu-id="7ab4c-152">Relationship</span></span> | <span data-ttu-id="7ab4c-153">类型</span><span class="sxs-lookup"><span data-stu-id="7ab4c-153">Type</span></span>   |<span data-ttu-id="7ab4c-154">说明</span><span class="sxs-lookup"><span data-stu-id="7ab4c-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ab4c-155">资源</span><span class="sxs-lookup"><span data-stu-id="7ab4c-155">resource</span></span>|[<span data-ttu-id="7ab4c-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="7ab4c-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="7ab4c-157">只读。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-157">Read-only.</span></span> <span data-ttu-id="7ab4c-158">相关联的角色定义的资源。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="7ab4c-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="7ab4c-159">roleSetting</span></span>|[<span data-ttu-id="7ab4c-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="7ab4c-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="7ab4c-161">角色定义关联的角色设置。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ab4c-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ab4c-162">JSON representation</span></span>

<span data-ttu-id="7ab4c-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ab4c-163">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

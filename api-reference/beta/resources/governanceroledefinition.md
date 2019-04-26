---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。
localization_priority: Normal
ms.openlocfilehash: 27b4b144f834f3b5eb4270a2875da5add10efb9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333748"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="4900f-104">governanceRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="4900f-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="4900f-105">表示角色定义。</span><span class="sxs-lookup"><span data-stu-id="4900f-105">Represents the role definitions.</span></span> <span data-ttu-id="4900f-106">对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。</span><span class="sxs-lookup"><span data-stu-id="4900f-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="4900f-107">方法</span><span class="sxs-lookup"><span data-stu-id="4900f-107">Methods</span></span>

| <span data-ttu-id="4900f-108">方法</span><span class="sxs-lookup"><span data-stu-id="4900f-108">Method</span></span>          | <span data-ttu-id="4900f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4900f-109">Return Type</span></span> |<span data-ttu-id="4900f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4900f-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="4900f-111">List</span><span class="sxs-lookup"><span data-stu-id="4900f-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="4900f-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="4900f-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="4900f-113">列出资源上的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="4900f-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="4900f-114">Get</span><span class="sxs-lookup"><span data-stu-id="4900f-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="4900f-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4900f-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="4900f-116">读取由 id 指定的角色定义实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4900f-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="4900f-117">目前`POST`, `PUT`entity `PATCH`set `DELETE`上`roleDefinitions`不支持,,,。</span><span class="sxs-lookup"><span data-stu-id="4900f-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="4900f-118">属性</span><span class="sxs-lookup"><span data-stu-id="4900f-118">Properties</span></span>
| <span data-ttu-id="4900f-119">属性</span><span class="sxs-lookup"><span data-stu-id="4900f-119">Property</span></span>  | <span data-ttu-id="4900f-120">类型</span><span class="sxs-lookup"><span data-stu-id="4900f-120">Type</span></span>      |<span data-ttu-id="4900f-121">说明</span><span class="sxs-lookup"><span data-stu-id="4900f-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="4900f-122">id</span><span class="sxs-lookup"><span data-stu-id="4900f-122">id</span></span>         |<span data-ttu-id="4900f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="4900f-123">String</span></span>     |<span data-ttu-id="4900f-124">角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="4900f-124">The id of the role definition.</span></span> |
|<span data-ttu-id="4900f-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="4900f-125">resourceId</span></span> |<span data-ttu-id="4900f-126">String</span><span class="sxs-lookup"><span data-stu-id="4900f-126">String</span></span>     |<span data-ttu-id="4900f-127">必需。</span><span class="sxs-lookup"><span data-stu-id="4900f-127">Required.</span></span> <span data-ttu-id="4900f-128">与角色定义关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="4900f-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="4900f-129">externalId</span><span class="sxs-lookup"><span data-stu-id="4900f-129">externalId</span></span>   |<span data-ttu-id="4900f-130">String</span><span class="sxs-lookup"><span data-stu-id="4900f-130">String</span></span>     |<span data-ttu-id="4900f-131">角色定义的外部 id。</span><span class="sxs-lookup"><span data-stu-id="4900f-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="4900f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4900f-132">displayName</span></span>|<span data-ttu-id="4900f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4900f-133">String</span></span>     |<span data-ttu-id="4900f-134">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4900f-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="4900f-135">templateId</span><span class="sxs-lookup"><span data-stu-id="4900f-135">templateId</span></span> | <span data-ttu-id="4900f-136">String</span><span class="sxs-lookup"><span data-stu-id="4900f-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="4900f-137">关系</span><span class="sxs-lookup"><span data-stu-id="4900f-137">Relationships</span></span>
| <span data-ttu-id="4900f-138">关系</span><span class="sxs-lookup"><span data-stu-id="4900f-138">Relationship</span></span> | <span data-ttu-id="4900f-139">类型</span><span class="sxs-lookup"><span data-stu-id="4900f-139">Type</span></span>   |<span data-ttu-id="4900f-140">说明</span><span class="sxs-lookup"><span data-stu-id="4900f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4900f-141">资源</span><span class="sxs-lookup"><span data-stu-id="4900f-141">resource</span></span>|[<span data-ttu-id="4900f-142">governanceResource</span><span class="sxs-lookup"><span data-stu-id="4900f-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="4900f-143">只读。</span><span class="sxs-lookup"><span data-stu-id="4900f-143">Read-only.</span></span> <span data-ttu-id="4900f-144">角色定义的关联资源。</span><span class="sxs-lookup"><span data-stu-id="4900f-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="4900f-145">roleSetting</span><span class="sxs-lookup"><span data-stu-id="4900f-145">roleSetting</span></span>|[<span data-ttu-id="4900f-146">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="4900f-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="4900f-147">角色定义的关联角色设置。</span><span class="sxs-lookup"><span data-stu-id="4900f-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4900f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4900f-148">JSON representation</span></span>

<span data-ttu-id="4900f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4900f-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "templateId":"String"
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
  "suppressions": []
}
-->

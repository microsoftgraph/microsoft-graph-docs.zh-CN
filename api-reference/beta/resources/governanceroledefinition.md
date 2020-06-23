---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 对于 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、读者、参与者等。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1435e8326536aa1a8943e46799d6a5612485a425
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845741"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="2c190-104">governanceRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c190-104">governanceRoleDefinition resource type</span></span>

<span data-ttu-id="2c190-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c190-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="2c190-106">表示角色定义。</span><span class="sxs-lookup"><span data-stu-id="2c190-106">Represents the role definitions.</span></span> <span data-ttu-id="2c190-107">对于 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、读者、参与者等。</span><span class="sxs-lookup"><span data-stu-id="2c190-107">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2c190-108">Methods</span><span class="sxs-lookup"><span data-stu-id="2c190-108">Methods</span></span>

| <span data-ttu-id="2c190-109">方法</span><span class="sxs-lookup"><span data-stu-id="2c190-109">Method</span></span>          | <span data-ttu-id="2c190-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c190-110">Return Type</span></span> |<span data-ttu-id="2c190-111">Description</span><span class="sxs-lookup"><span data-stu-id="2c190-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="2c190-112">List</span><span class="sxs-lookup"><span data-stu-id="2c190-112">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="2c190-113">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c190-113">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="2c190-114">列出资源上的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="2c190-114">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="2c190-115">获取</span><span class="sxs-lookup"><span data-stu-id="2c190-115">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="2c190-116">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2c190-116">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="2c190-117">读取由 id 指定的角色定义实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c190-117">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="2c190-118">`POST`目前， `PUT` `PATCH` `DELETE` entity set 上不支持，，， `roleDefinitions` 。</span><span class="sxs-lookup"><span data-stu-id="2c190-118">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="2c190-119">属性</span><span class="sxs-lookup"><span data-stu-id="2c190-119">Properties</span></span>
| <span data-ttu-id="2c190-120">属性</span><span class="sxs-lookup"><span data-stu-id="2c190-120">Property</span></span>    | <span data-ttu-id="2c190-121">类型</span><span class="sxs-lookup"><span data-stu-id="2c190-121">Type</span></span>   | <span data-ttu-id="2c190-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c190-122">Description</span></span>                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| <span data-ttu-id="2c190-123">id</span><span class="sxs-lookup"><span data-stu-id="2c190-123">id</span></span>          | <span data-ttu-id="2c190-124">字符串</span><span class="sxs-lookup"><span data-stu-id="2c190-124">String</span></span> | <span data-ttu-id="2c190-125">角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="2c190-125">The id of the role definition.</span></span>                                        |
| <span data-ttu-id="2c190-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="2c190-126">resourceId</span></span>  | <span data-ttu-id="2c190-127">String</span><span class="sxs-lookup"><span data-stu-id="2c190-127">String</span></span> | <span data-ttu-id="2c190-128">必填。</span><span class="sxs-lookup"><span data-stu-id="2c190-128">Required.</span></span> <span data-ttu-id="2c190-129">与角色定义关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="2c190-129">The id of the resource associated with the role definition.</span></span> |
| <span data-ttu-id="2c190-130">externalId</span><span class="sxs-lookup"><span data-stu-id="2c190-130">externalId</span></span>  | <span data-ttu-id="2c190-131">String</span><span class="sxs-lookup"><span data-stu-id="2c190-131">String</span></span> | <span data-ttu-id="2c190-132">角色定义的外部 id。</span><span class="sxs-lookup"><span data-stu-id="2c190-132">The external id of the role definition.</span></span>                               |
| <span data-ttu-id="2c190-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2c190-133">displayName</span></span> | <span data-ttu-id="2c190-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2c190-134">String</span></span> | <span data-ttu-id="2c190-135">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2c190-135">The display name of the role definition.</span></span>                              |
| <span data-ttu-id="2c190-136">templateId</span><span class="sxs-lookup"><span data-stu-id="2c190-136">templateId</span></span>  | <span data-ttu-id="2c190-137">String</span><span class="sxs-lookup"><span data-stu-id="2c190-137">String</span></span> |                                                                       |

## <a name="relationships"></a><span data-ttu-id="2c190-138">关系</span><span class="sxs-lookup"><span data-stu-id="2c190-138">Relationships</span></span>
| <span data-ttu-id="2c190-139">关系</span><span class="sxs-lookup"><span data-stu-id="2c190-139">Relationship</span></span> | <span data-ttu-id="2c190-140">类型</span><span class="sxs-lookup"><span data-stu-id="2c190-140">Type</span></span>   |<span data-ttu-id="2c190-141">说明</span><span class="sxs-lookup"><span data-stu-id="2c190-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c190-142">资源</span><span class="sxs-lookup"><span data-stu-id="2c190-142">resource</span></span>|[<span data-ttu-id="2c190-143">governanceResource</span><span class="sxs-lookup"><span data-stu-id="2c190-143">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="2c190-144">只读。</span><span class="sxs-lookup"><span data-stu-id="2c190-144">Read-only.</span></span> <span data-ttu-id="2c190-145">角色定义的关联资源。</span><span class="sxs-lookup"><span data-stu-id="2c190-145">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="2c190-146">roleSetting</span><span class="sxs-lookup"><span data-stu-id="2c190-146">roleSetting</span></span>|[<span data-ttu-id="2c190-147">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="2c190-147">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="2c190-148">角色定义的关联角色设置。</span><span class="sxs-lookup"><span data-stu-id="2c190-148">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c190-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c190-149">JSON representation</span></span>

<span data-ttu-id="2c190-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c190-150">Here is a JSON representation of the resource.</span></span>

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

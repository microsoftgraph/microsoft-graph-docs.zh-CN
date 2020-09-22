---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d004572b1cf07fdbd09cce585579cf2c8ed57541
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043876"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="a6006-106">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6006-106">roleAssignment resource type</span></span>

<span data-ttu-id="a6006-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6006-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6006-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6006-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6006-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="a6006-109">The Role Assignment resource.</span></span> <span data-ttu-id="a6006-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="a6006-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="a6006-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="a6006-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="a6006-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="a6006-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="a6006-113">方法</span><span class="sxs-lookup"><span data-stu-id="a6006-113">Methods</span></span>
|<span data-ttu-id="a6006-114">方法</span><span class="sxs-lookup"><span data-stu-id="a6006-114">Method</span></span>|<span data-ttu-id="a6006-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6006-115">Return Type</span></span>|<span data-ttu-id="a6006-116">说明</span><span class="sxs-lookup"><span data-stu-id="a6006-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6006-117">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a6006-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="a6006-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6006-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="a6006-119">列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6006-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="a6006-120">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="a6006-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6006-122">读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6006-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a6006-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="a6006-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6006-125">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6006-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a6006-126">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="a6006-127">无</span><span class="sxs-lookup"><span data-stu-id="a6006-127">None</span></span>|<span data-ttu-id="a6006-128">删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a6006-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="a6006-129">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="a6006-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6006-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6006-131">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6006-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6006-132">属性</span><span class="sxs-lookup"><span data-stu-id="a6006-132">Properties</span></span>
|<span data-ttu-id="a6006-133">属性</span><span class="sxs-lookup"><span data-stu-id="a6006-133">Property</span></span>|<span data-ttu-id="a6006-134">类型</span><span class="sxs-lookup"><span data-stu-id="a6006-134">Type</span></span>|<span data-ttu-id="a6006-135">说明</span><span class="sxs-lookup"><span data-stu-id="a6006-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6006-136">id</span><span class="sxs-lookup"><span data-stu-id="a6006-136">id</span></span>|<span data-ttu-id="a6006-137">String</span><span class="sxs-lookup"><span data-stu-id="a6006-137">String</span></span>|<span data-ttu-id="a6006-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6006-138">Key of the entity.</span></span> <span data-ttu-id="a6006-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a6006-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a6006-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a6006-140">displayName</span></span>|<span data-ttu-id="a6006-141">String</span><span class="sxs-lookup"><span data-stu-id="a6006-141">String</span></span>|<span data-ttu-id="a6006-142">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a6006-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a6006-143">description</span><span class="sxs-lookup"><span data-stu-id="a6006-143">description</span></span>|<span data-ttu-id="a6006-144">String</span><span class="sxs-lookup"><span data-stu-id="a6006-144">String</span></span>|<span data-ttu-id="a6006-145">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="a6006-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a6006-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a6006-146">resourceScopes</span></span>|<span data-ttu-id="a6006-147">String collection</span><span class="sxs-lookup"><span data-stu-id="a6006-147">String collection</span></span>|<span data-ttu-id="a6006-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a6006-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a6006-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6006-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6006-150">关系</span><span class="sxs-lookup"><span data-stu-id="a6006-150">Relationships</span></span>
|<span data-ttu-id="a6006-151">关系</span><span class="sxs-lookup"><span data-stu-id="a6006-151">Relationship</span></span>|<span data-ttu-id="a6006-152">类型</span><span class="sxs-lookup"><span data-stu-id="a6006-152">Type</span></span>|<span data-ttu-id="a6006-153">说明</span><span class="sxs-lookup"><span data-stu-id="a6006-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6006-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6006-154">roleDefinition</span></span>|[<span data-ttu-id="a6006-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6006-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a6006-156">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="a6006-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6006-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6006-157">JSON Representation</span></span>
<span data-ttu-id="a6006-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6006-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```










---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b388c043a1903394b1525c10eda7e817f1f1fdf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441599"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="8506f-106">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8506f-106">roleAssignment resource type</span></span>

<span data-ttu-id="8506f-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8506f-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8506f-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8506f-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8506f-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="8506f-109">The Role Assignment resource.</span></span> <span data-ttu-id="8506f-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="8506f-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="8506f-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="8506f-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="8506f-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="8506f-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="8506f-113">方法</span><span class="sxs-lookup"><span data-stu-id="8506f-113">Methods</span></span>
|<span data-ttu-id="8506f-114">方法</span><span class="sxs-lookup"><span data-stu-id="8506f-114">Method</span></span>|<span data-ttu-id="8506f-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="8506f-115">Return Type</span></span>|<span data-ttu-id="8506f-116">说明</span><span class="sxs-lookup"><span data-stu-id="8506f-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8506f-117">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="8506f-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="8506f-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8506f-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="8506f-119">列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8506f-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="8506f-120">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="8506f-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="8506f-122">读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8506f-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="8506f-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="8506f-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="8506f-125">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8506f-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="8506f-126">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="8506f-127">无</span><span class="sxs-lookup"><span data-stu-id="8506f-127">None</span></span>|<span data-ttu-id="8506f-128">删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="8506f-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="8506f-129">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="8506f-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8506f-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="8506f-131">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8506f-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8506f-132">属性</span><span class="sxs-lookup"><span data-stu-id="8506f-132">Properties</span></span>
|<span data-ttu-id="8506f-133">属性</span><span class="sxs-lookup"><span data-stu-id="8506f-133">Property</span></span>|<span data-ttu-id="8506f-134">类型</span><span class="sxs-lookup"><span data-stu-id="8506f-134">Type</span></span>|<span data-ttu-id="8506f-135">说明</span><span class="sxs-lookup"><span data-stu-id="8506f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8506f-136">id</span><span class="sxs-lookup"><span data-stu-id="8506f-136">id</span></span>|<span data-ttu-id="8506f-137">字符串</span><span class="sxs-lookup"><span data-stu-id="8506f-137">String</span></span>|<span data-ttu-id="8506f-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8506f-138">Key of the entity.</span></span> <span data-ttu-id="8506f-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="8506f-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8506f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8506f-140">displayName</span></span>|<span data-ttu-id="8506f-141">String</span><span class="sxs-lookup"><span data-stu-id="8506f-141">String</span></span>|<span data-ttu-id="8506f-142">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="8506f-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="8506f-143">description</span><span class="sxs-lookup"><span data-stu-id="8506f-143">description</span></span>|<span data-ttu-id="8506f-144">String</span><span class="sxs-lookup"><span data-stu-id="8506f-144">String</span></span>|<span data-ttu-id="8506f-145">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="8506f-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="8506f-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="8506f-146">resourceScopes</span></span>|<span data-ttu-id="8506f-147">String collection</span><span class="sxs-lookup"><span data-stu-id="8506f-147">String collection</span></span>|<span data-ttu-id="8506f-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="8506f-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="8506f-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="8506f-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8506f-150">关系</span><span class="sxs-lookup"><span data-stu-id="8506f-150">Relationships</span></span>
|<span data-ttu-id="8506f-151">关系</span><span class="sxs-lookup"><span data-stu-id="8506f-151">Relationship</span></span>|<span data-ttu-id="8506f-152">类型</span><span class="sxs-lookup"><span data-stu-id="8506f-152">Type</span></span>|<span data-ttu-id="8506f-153">说明</span><span class="sxs-lookup"><span data-stu-id="8506f-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8506f-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8506f-154">roleDefinition</span></span>|[<span data-ttu-id="8506f-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8506f-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="8506f-156">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="8506f-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8506f-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8506f-157">JSON Representation</span></span>
<span data-ttu-id="8506f-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8506f-158">Here is a JSON representation of the resource.</span></span>
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








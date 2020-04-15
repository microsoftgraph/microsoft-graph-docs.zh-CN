---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84a4999e2738d4b068daf88e97896c418f2db6b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441659"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="5f192-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f192-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="5f192-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f192-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f192-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f192-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f192-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="5f192-109">The Role Assignment resource.</span></span> <span data-ttu-id="5f192-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="5f192-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="5f192-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="5f192-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="5f192-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="5f192-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="5f192-113">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5f192-114">方法</span><span class="sxs-lookup"><span data-stu-id="5f192-114">Methods</span></span>
|<span data-ttu-id="5f192-115">方法</span><span class="sxs-lookup"><span data-stu-id="5f192-115">Method</span></span>|<span data-ttu-id="5f192-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f192-116">Return Type</span></span>|<span data-ttu-id="5f192-117">说明</span><span class="sxs-lookup"><span data-stu-id="5f192-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f192-118">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="5f192-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="5f192-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f192-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="5f192-120">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f192-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="5f192-121">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="5f192-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5f192-123">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f192-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="5f192-124">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="5f192-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5f192-126">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f192-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="5f192-127">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="5f192-128">无</span><span class="sxs-lookup"><span data-stu-id="5f192-128">None</span></span>|<span data-ttu-id="5f192-129">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5f192-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="5f192-130">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="5f192-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f192-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5f192-132">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5f192-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f192-133">属性</span><span class="sxs-lookup"><span data-stu-id="5f192-133">Properties</span></span>
|<span data-ttu-id="5f192-134">属性</span><span class="sxs-lookup"><span data-stu-id="5f192-134">Property</span></span>|<span data-ttu-id="5f192-135">类型</span><span class="sxs-lookup"><span data-stu-id="5f192-135">Type</span></span>|<span data-ttu-id="5f192-136">说明</span><span class="sxs-lookup"><span data-stu-id="5f192-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f192-137">id</span><span class="sxs-lookup"><span data-stu-id="5f192-137">id</span></span>|<span data-ttu-id="5f192-138">字符串</span><span class="sxs-lookup"><span data-stu-id="5f192-138">String</span></span>|<span data-ttu-id="5f192-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5f192-139">Key of the entity.</span></span> <span data-ttu-id="5f192-140">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="5f192-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="5f192-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5f192-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5f192-142">displayName</span></span>|<span data-ttu-id="5f192-143">String</span><span class="sxs-lookup"><span data-stu-id="5f192-143">String</span></span>|<span data-ttu-id="5f192-144">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="5f192-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="5f192-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5f192-146">description</span><span class="sxs-lookup"><span data-stu-id="5f192-146">description</span></span>|<span data-ttu-id="5f192-147">String</span><span class="sxs-lookup"><span data-stu-id="5f192-147">String</span></span>|<span data-ttu-id="5f192-148">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="5f192-148">Description of the Role Assignment.</span></span> <span data-ttu-id="5f192-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5f192-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5f192-150">resourceScopes</span></span>|<span data-ttu-id="5f192-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="5f192-151">String collection</span></span>|<span data-ttu-id="5f192-152">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5f192-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5f192-153">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="5f192-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5f192-154">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5f192-155">members</span><span class="sxs-lookup"><span data-stu-id="5f192-155">members</span></span>|<span data-ttu-id="5f192-156">String collection</span><span class="sxs-lookup"><span data-stu-id="5f192-156">String collection</span></span>|<span data-ttu-id="5f192-157">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5f192-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="5f192-158">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5f192-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f192-159">关系</span><span class="sxs-lookup"><span data-stu-id="5f192-159">Relationships</span></span>
|<span data-ttu-id="5f192-160">关系</span><span class="sxs-lookup"><span data-stu-id="5f192-160">Relationship</span></span>|<span data-ttu-id="5f192-161">类型</span><span class="sxs-lookup"><span data-stu-id="5f192-161">Type</span></span>|<span data-ttu-id="5f192-162">说明</span><span class="sxs-lookup"><span data-stu-id="5f192-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f192-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5f192-163">roleDefinition</span></span>|[<span data-ttu-id="5f192-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5f192-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5f192-165">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="5f192-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="5f192-166">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f192-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f192-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f192-167">JSON Representation</span></span>
<span data-ttu-id="5f192-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f192-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```








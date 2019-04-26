---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfbb4e3b51f56e447ba69caefbf2b0b5226a5d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567485"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="297be-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="297be-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="297be-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="297be-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="297be-108">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="297be-108">The Role Assignment resource.</span></span> <span data-ttu-id="297be-109">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="297be-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="297be-110">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="297be-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="297be-111">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="297be-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="297be-112">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="297be-113">方法</span><span class="sxs-lookup"><span data-stu-id="297be-113">Methods</span></span>
|<span data-ttu-id="297be-114">方法</span><span class="sxs-lookup"><span data-stu-id="297be-114">Method</span></span>|<span data-ttu-id="297be-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="297be-115">Return Type</span></span>|<span data-ttu-id="297be-116">说明</span><span class="sxs-lookup"><span data-stu-id="297be-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="297be-117">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="297be-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="297be-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="297be-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="297be-119">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="297be-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="297be-120">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="297be-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="297be-122">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="297be-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="297be-123">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="297be-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="297be-125">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="297be-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="297be-126">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="297be-127">无</span><span class="sxs-lookup"><span data-stu-id="297be-127">None</span></span>|<span data-ttu-id="297be-128">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="297be-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="297be-129">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="297be-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="297be-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="297be-131">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="297be-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="297be-132">属性</span><span class="sxs-lookup"><span data-stu-id="297be-132">Properties</span></span>
|<span data-ttu-id="297be-133">属性</span><span class="sxs-lookup"><span data-stu-id="297be-133">Property</span></span>|<span data-ttu-id="297be-134">类型</span><span class="sxs-lookup"><span data-stu-id="297be-134">Type</span></span>|<span data-ttu-id="297be-135">说明</span><span class="sxs-lookup"><span data-stu-id="297be-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297be-136">id</span><span class="sxs-lookup"><span data-stu-id="297be-136">id</span></span>|<span data-ttu-id="297be-137">字符串</span><span class="sxs-lookup"><span data-stu-id="297be-137">String</span></span>|<span data-ttu-id="297be-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="297be-138">Key of the entity.</span></span> <span data-ttu-id="297be-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="297be-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="297be-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="297be-141">displayName</span><span class="sxs-lookup"><span data-stu-id="297be-141">displayName</span></span>|<span data-ttu-id="297be-142">String</span><span class="sxs-lookup"><span data-stu-id="297be-142">String</span></span>|<span data-ttu-id="297be-143">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="297be-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="297be-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="297be-145">说明</span><span class="sxs-lookup"><span data-stu-id="297be-145">description</span></span>|<span data-ttu-id="297be-146">String</span><span class="sxs-lookup"><span data-stu-id="297be-146">String</span></span>|<span data-ttu-id="297be-147">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="297be-147">Description of the Role Assignment.</span></span> <span data-ttu-id="297be-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="297be-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="297be-149">resourceScopes</span></span>|<span data-ttu-id="297be-150">String collection</span><span class="sxs-lookup"><span data-stu-id="297be-150">String collection</span></span>|<span data-ttu-id="297be-151">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="297be-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="297be-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="297be-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="297be-153">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="297be-154">members</span><span class="sxs-lookup"><span data-stu-id="297be-154">members</span></span>|<span data-ttu-id="297be-155">String collection</span><span class="sxs-lookup"><span data-stu-id="297be-155">String collection</span></span>|<span data-ttu-id="297be-156">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="297be-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="297be-157">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="297be-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="297be-158">关系</span><span class="sxs-lookup"><span data-stu-id="297be-158">Relationships</span></span>
|<span data-ttu-id="297be-159">关系</span><span class="sxs-lookup"><span data-stu-id="297be-159">Relationship</span></span>|<span data-ttu-id="297be-160">类型</span><span class="sxs-lookup"><span data-stu-id="297be-160">Type</span></span>|<span data-ttu-id="297be-161">说明</span><span class="sxs-lookup"><span data-stu-id="297be-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297be-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="297be-162">roleDefinition</span></span>|[<span data-ttu-id="297be-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="297be-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="297be-164">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="297be-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="297be-165">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="297be-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="297be-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="297be-166">JSON Representation</span></span>
<span data-ttu-id="297be-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="297be-167">Here is a JSON representation of the resource.</span></span>
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




---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bab20156891a637c0cb62aa0f1439b19c103a1d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447967"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="c37b8-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c37b8-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="c37b8-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c37b8-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c37b8-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c37b8-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c37b8-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="c37b8-109">The Role Assignment resource.</span></span> <span data-ttu-id="c37b8-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="c37b8-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="c37b8-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="c37b8-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="c37b8-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="c37b8-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="c37b8-113">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c37b8-114">方法</span><span class="sxs-lookup"><span data-stu-id="c37b8-114">Methods</span></span>
|<span data-ttu-id="c37b8-115">方法</span><span class="sxs-lookup"><span data-stu-id="c37b8-115">Method</span></span>|<span data-ttu-id="c37b8-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="c37b8-116">Return Type</span></span>|<span data-ttu-id="c37b8-117">说明</span><span class="sxs-lookup"><span data-stu-id="c37b8-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c37b8-118">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="c37b8-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="c37b8-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c37b8-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="c37b8-120">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c37b8-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="c37b8-121">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="c37b8-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="c37b8-123">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c37b8-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="c37b8-124">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="c37b8-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="c37b8-126">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c37b8-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="c37b8-127">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="c37b8-128">无</span><span class="sxs-lookup"><span data-stu-id="c37b8-128">None</span></span>|<span data-ttu-id="c37b8-129">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c37b8-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="c37b8-130">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="c37b8-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c37b8-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="c37b8-132">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c37b8-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c37b8-133">属性</span><span class="sxs-lookup"><span data-stu-id="c37b8-133">Properties</span></span>
|<span data-ttu-id="c37b8-134">属性</span><span class="sxs-lookup"><span data-stu-id="c37b8-134">Property</span></span>|<span data-ttu-id="c37b8-135">类型</span><span class="sxs-lookup"><span data-stu-id="c37b8-135">Type</span></span>|<span data-ttu-id="c37b8-136">说明</span><span class="sxs-lookup"><span data-stu-id="c37b8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37b8-137">id</span><span class="sxs-lookup"><span data-stu-id="c37b8-137">id</span></span>|<span data-ttu-id="c37b8-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c37b8-138">String</span></span>|<span data-ttu-id="c37b8-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c37b8-139">Key of the entity.</span></span> <span data-ttu-id="c37b8-140">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="c37b8-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="c37b8-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c37b8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c37b8-142">displayName</span></span>|<span data-ttu-id="c37b8-143">String</span><span class="sxs-lookup"><span data-stu-id="c37b8-143">String</span></span>|<span data-ttu-id="c37b8-144">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="c37b8-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="c37b8-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c37b8-146">说明</span><span class="sxs-lookup"><span data-stu-id="c37b8-146">description</span></span>|<span data-ttu-id="c37b8-147">String</span><span class="sxs-lookup"><span data-stu-id="c37b8-147">String</span></span>|<span data-ttu-id="c37b8-148">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="c37b8-148">Description of the Role Assignment.</span></span> <span data-ttu-id="c37b8-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c37b8-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c37b8-150">resourceScopes</span></span>|<span data-ttu-id="c37b8-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="c37b8-151">String collection</span></span>|<span data-ttu-id="c37b8-152">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="c37b8-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c37b8-153">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="c37b8-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="c37b8-154">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c37b8-155">members</span><span class="sxs-lookup"><span data-stu-id="c37b8-155">members</span></span>|<span data-ttu-id="c37b8-156">String collection</span><span class="sxs-lookup"><span data-stu-id="c37b8-156">String collection</span></span>|<span data-ttu-id="c37b8-157">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="c37b8-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="c37b8-158">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="c37b8-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c37b8-159">关系</span><span class="sxs-lookup"><span data-stu-id="c37b8-159">Relationships</span></span>
|<span data-ttu-id="c37b8-160">关系</span><span class="sxs-lookup"><span data-stu-id="c37b8-160">Relationship</span></span>|<span data-ttu-id="c37b8-161">类型</span><span class="sxs-lookup"><span data-stu-id="c37b8-161">Type</span></span>|<span data-ttu-id="c37b8-162">说明</span><span class="sxs-lookup"><span data-stu-id="c37b8-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37b8-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c37b8-163">roleDefinition</span></span>|[<span data-ttu-id="c37b8-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c37b8-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="c37b8-165">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="c37b8-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="c37b8-166">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c37b8-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c37b8-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c37b8-167">JSON Representation</span></span>
<span data-ttu-id="c37b8-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c37b8-168">Here is a JSON representation of the resource.</span></span>
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





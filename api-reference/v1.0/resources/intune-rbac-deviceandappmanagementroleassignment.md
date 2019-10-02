---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9cd47a62afeb625ca4ea6aeeaea531307a490b2e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360823"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="a7a3f-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7a3f-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="a7a3f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7a3f-108">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-108">The Role Assignment resource.</span></span> <span data-ttu-id="a7a3f-109">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="a7a3f-110">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="a7a3f-111">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="a7a3f-112">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a7a3f-113">方法</span><span class="sxs-lookup"><span data-stu-id="a7a3f-113">Methods</span></span>
|<span data-ttu-id="a7a3f-114">方法</span><span class="sxs-lookup"><span data-stu-id="a7a3f-114">Method</span></span>|<span data-ttu-id="a7a3f-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7a3f-115">Return Type</span></span>|<span data-ttu-id="a7a3f-116">说明</span><span class="sxs-lookup"><span data-stu-id="a7a3f-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7a3f-117">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="a7a3f-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="a7a3f-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7a3f-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="a7a3f-119">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="a7a3f-120">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="a7a3f-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="a7a3f-122">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="a7a3f-123">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="a7a3f-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="a7a3f-125">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="a7a3f-126">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="a7a3f-127">无</span><span class="sxs-lookup"><span data-stu-id="a7a3f-127">None</span></span>|<span data-ttu-id="a7a3f-128">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="a7a3f-129">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="a7a3f-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a7a3f-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="a7a3f-131">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7a3f-132">属性</span><span class="sxs-lookup"><span data-stu-id="a7a3f-132">Properties</span></span>
|<span data-ttu-id="a7a3f-133">属性</span><span class="sxs-lookup"><span data-stu-id="a7a3f-133">Property</span></span>|<span data-ttu-id="a7a3f-134">类型</span><span class="sxs-lookup"><span data-stu-id="a7a3f-134">Type</span></span>|<span data-ttu-id="a7a3f-135">说明</span><span class="sxs-lookup"><span data-stu-id="a7a3f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a3f-136">id</span><span class="sxs-lookup"><span data-stu-id="a7a3f-136">id</span></span>|<span data-ttu-id="a7a3f-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a7a3f-137">String</span></span>|<span data-ttu-id="a7a3f-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-138">Key of the entity.</span></span> <span data-ttu-id="a7a3f-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="a7a3f-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a7a3f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a7a3f-141">displayName</span></span>|<span data-ttu-id="a7a3f-142">String</span><span class="sxs-lookup"><span data-stu-id="a7a3f-142">String</span></span>|<span data-ttu-id="a7a3f-143">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="a7a3f-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a7a3f-145">说明</span><span class="sxs-lookup"><span data-stu-id="a7a3f-145">description</span></span>|<span data-ttu-id="a7a3f-146">String</span><span class="sxs-lookup"><span data-stu-id="a7a3f-146">String</span></span>|<span data-ttu-id="a7a3f-147">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-147">Description of the Role Assignment.</span></span> <span data-ttu-id="a7a3f-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a7a3f-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a7a3f-149">resourceScopes</span></span>|<span data-ttu-id="a7a3f-150">String collection</span><span class="sxs-lookup"><span data-stu-id="a7a3f-150">String collection</span></span>|<span data-ttu-id="a7a3f-151">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a7a3f-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="a7a3f-153">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a7a3f-154">members</span><span class="sxs-lookup"><span data-stu-id="a7a3f-154">members</span></span>|<span data-ttu-id="a7a3f-155">String collection</span><span class="sxs-lookup"><span data-stu-id="a7a3f-155">String collection</span></span>|<span data-ttu-id="a7a3f-156">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="a7a3f-157">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7a3f-158">关系</span><span class="sxs-lookup"><span data-stu-id="a7a3f-158">Relationships</span></span>
|<span data-ttu-id="a7a3f-159">关系</span><span class="sxs-lookup"><span data-stu-id="a7a3f-159">Relationship</span></span>|<span data-ttu-id="a7a3f-160">类型</span><span class="sxs-lookup"><span data-stu-id="a7a3f-160">Type</span></span>|<span data-ttu-id="a7a3f-161">说明</span><span class="sxs-lookup"><span data-stu-id="a7a3f-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a3f-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a7a3f-162">roleDefinition</span></span>|[<span data-ttu-id="a7a3f-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a7a3f-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a7a3f-164">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="a7a3f-165">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7a3f-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7a3f-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7a3f-166">JSON Representation</span></span>
<span data-ttu-id="a7a3f-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7a3f-167">Here is a JSON representation of the resource.</span></span>
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





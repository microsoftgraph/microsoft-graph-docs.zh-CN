---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
ms.openlocfilehash: 23300e40afab6edd2033857e828ea0f65e52d604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309308"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="9db9d-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db9d-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="9db9d-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9db9d-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9db9d-108">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="9db9d-108">The Role Assignment resource.</span></span> <span data-ttu-id="9db9d-109">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="9db9d-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="9db9d-110">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="9db9d-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="9db9d-111">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="9db9d-111">This applies to custom and built-in roles.</span></span>

<span data-ttu-id="9db9d-112">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9db9d-113">方法</span><span class="sxs-lookup"><span data-stu-id="9db9d-113">Methods</span></span>
|<span data-ttu-id="9db9d-114">方法</span><span class="sxs-lookup"><span data-stu-id="9db9d-114">Method</span></span>|<span data-ttu-id="9db9d-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="9db9d-115">Return Type</span></span>|<span data-ttu-id="9db9d-116">说明</span><span class="sxs-lookup"><span data-stu-id="9db9d-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9db9d-117">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="9db9d-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="9db9d-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9db9d-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="9db9d-119">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9db9d-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="9db9d-120">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="9db9d-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="9db9d-122">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9db9d-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="9db9d-123">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="9db9d-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="9db9d-125">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9db9d-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="9db9d-126">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="9db9d-127">无</span><span class="sxs-lookup"><span data-stu-id="9db9d-127">None</span></span>|<span data-ttu-id="9db9d-128">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="9db9d-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="9db9d-129">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="9db9d-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9db9d-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="9db9d-131">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9db9d-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9db9d-132">属性</span><span class="sxs-lookup"><span data-stu-id="9db9d-132">Properties</span></span>
|<span data-ttu-id="9db9d-133">属性</span><span class="sxs-lookup"><span data-stu-id="9db9d-133">Property</span></span>|<span data-ttu-id="9db9d-134">类型</span><span class="sxs-lookup"><span data-stu-id="9db9d-134">Type</span></span>|<span data-ttu-id="9db9d-135">说明</span><span class="sxs-lookup"><span data-stu-id="9db9d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db9d-136">id</span><span class="sxs-lookup"><span data-stu-id="9db9d-136">id</span></span>|<span data-ttu-id="9db9d-137">String</span><span class="sxs-lookup"><span data-stu-id="9db9d-137">String</span></span>|<span data-ttu-id="9db9d-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9db9d-138">Key of the entity.</span></span> <span data-ttu-id="9db9d-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="9db9d-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="9db9d-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9db9d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="9db9d-141">displayName</span></span>|<span data-ttu-id="9db9d-142">String</span><span class="sxs-lookup"><span data-stu-id="9db9d-142">String</span></span>|<span data-ttu-id="9db9d-143">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="9db9d-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="9db9d-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9db9d-145">description</span><span class="sxs-lookup"><span data-stu-id="9db9d-145">description</span></span>|<span data-ttu-id="9db9d-146">String</span><span class="sxs-lookup"><span data-stu-id="9db9d-146">String</span></span>|<span data-ttu-id="9db9d-147">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="9db9d-147">Description of the Role Assignment.</span></span> <span data-ttu-id="9db9d-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9db9d-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9db9d-149">resourceScopes</span></span>|<span data-ttu-id="9db9d-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="9db9d-150">String collection</span></span>|<span data-ttu-id="9db9d-151">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9db9d-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9db9d-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="9db9d-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="9db9d-153">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9db9d-154">members</span><span class="sxs-lookup"><span data-stu-id="9db9d-154">members</span></span>|<span data-ttu-id="9db9d-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="9db9d-155">String collection</span></span>|<span data-ttu-id="9db9d-156">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9db9d-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="9db9d-157">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="9db9d-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9db9d-158">关系</span><span class="sxs-lookup"><span data-stu-id="9db9d-158">Relationships</span></span>
|<span data-ttu-id="9db9d-159">关系</span><span class="sxs-lookup"><span data-stu-id="9db9d-159">Relationship</span></span>|<span data-ttu-id="9db9d-160">类型</span><span class="sxs-lookup"><span data-stu-id="9db9d-160">Type</span></span>|<span data-ttu-id="9db9d-161">说明</span><span class="sxs-lookup"><span data-stu-id="9db9d-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db9d-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9db9d-162">roleDefinition</span></span>|[<span data-ttu-id="9db9d-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9db9d-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="9db9d-164">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="9db9d-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="9db9d-165">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9db9d-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9db9d-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9db9d-166">JSON Representation</span></span>
<span data-ttu-id="9db9d-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db9d-167">Here is a JSON representation of the resource.</span></span>
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




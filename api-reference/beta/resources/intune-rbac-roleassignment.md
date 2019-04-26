---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cffebe54ba79d9b013068b9162f9e3a17447b15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566353"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="11c06-106">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="11c06-106">roleAssignment resource type</span></span>

> <span data-ttu-id="11c06-107">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11c06-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11c06-108">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11c06-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11c06-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="11c06-109">The Role Assignment resource.</span></span> <span data-ttu-id="11c06-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="11c06-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="11c06-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="11c06-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="11c06-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="11c06-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="11c06-113">方法</span><span class="sxs-lookup"><span data-stu-id="11c06-113">Methods</span></span>
|<span data-ttu-id="11c06-114">方法</span><span class="sxs-lookup"><span data-stu-id="11c06-114">Method</span></span>|<span data-ttu-id="11c06-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="11c06-115">Return Type</span></span>|<span data-ttu-id="11c06-116">说明</span><span class="sxs-lookup"><span data-stu-id="11c06-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11c06-117">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="11c06-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="11c06-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="11c06-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="11c06-119">列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11c06-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="11c06-120">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="11c06-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="11c06-122">读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11c06-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="11c06-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="11c06-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="11c06-125">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="11c06-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="11c06-126">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="11c06-127">无</span><span class="sxs-lookup"><span data-stu-id="11c06-127">None</span></span>|<span data-ttu-id="11c06-128">删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="11c06-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="11c06-129">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="11c06-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="11c06-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="11c06-131">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11c06-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11c06-132">属性</span><span class="sxs-lookup"><span data-stu-id="11c06-132">Properties</span></span>
|<span data-ttu-id="11c06-133">属性</span><span class="sxs-lookup"><span data-stu-id="11c06-133">Property</span></span>|<span data-ttu-id="11c06-134">类型</span><span class="sxs-lookup"><span data-stu-id="11c06-134">Type</span></span>|<span data-ttu-id="11c06-135">说明</span><span class="sxs-lookup"><span data-stu-id="11c06-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c06-136">id</span><span class="sxs-lookup"><span data-stu-id="11c06-136">id</span></span>|<span data-ttu-id="11c06-137">字符串</span><span class="sxs-lookup"><span data-stu-id="11c06-137">String</span></span>|<span data-ttu-id="11c06-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="11c06-138">Key of the entity.</span></span> <span data-ttu-id="11c06-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="11c06-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="11c06-140">displayName</span><span class="sxs-lookup"><span data-stu-id="11c06-140">displayName</span></span>|<span data-ttu-id="11c06-141">String</span><span class="sxs-lookup"><span data-stu-id="11c06-141">String</span></span>|<span data-ttu-id="11c06-142">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="11c06-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="11c06-143">说明</span><span class="sxs-lookup"><span data-stu-id="11c06-143">description</span></span>|<span data-ttu-id="11c06-144">String</span><span class="sxs-lookup"><span data-stu-id="11c06-144">String</span></span>|<span data-ttu-id="11c06-145">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="11c06-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="11c06-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="11c06-146">scopeMembers</span></span>|<span data-ttu-id="11c06-147">String collection</span><span class="sxs-lookup"><span data-stu-id="11c06-147">String collection</span></span>|<span data-ttu-id="11c06-148">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="11c06-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="11c06-149">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="11c06-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="11c06-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="11c06-150">scopeType</span></span>|[<span data-ttu-id="11c06-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="11c06-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="11c06-152">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="11c06-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="11c06-153">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="11c06-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="11c06-154">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="11c06-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="11c06-155">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="11c06-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="11c06-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="11c06-156">resourceScopes</span></span>|<span data-ttu-id="11c06-157">String collection</span><span class="sxs-lookup"><span data-stu-id="11c06-157">String collection</span></span>|<span data-ttu-id="11c06-158">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="11c06-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="11c06-159">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="11c06-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11c06-160">关系</span><span class="sxs-lookup"><span data-stu-id="11c06-160">Relationships</span></span>
|<span data-ttu-id="11c06-161">关系</span><span class="sxs-lookup"><span data-stu-id="11c06-161">Relationship</span></span>|<span data-ttu-id="11c06-162">类型</span><span class="sxs-lookup"><span data-stu-id="11c06-162">Type</span></span>|<span data-ttu-id="11c06-163">说明</span><span class="sxs-lookup"><span data-stu-id="11c06-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c06-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="11c06-164">roleDefinition</span></span>|[<span data-ttu-id="11c06-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="11c06-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="11c06-166">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="11c06-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11c06-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11c06-167">JSON Representation</span></span>
<span data-ttu-id="11c06-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11c06-168">Here is a JSON representation of the resource.</span></span>
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
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```






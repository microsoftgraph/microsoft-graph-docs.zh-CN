---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b766aed45d6725b6de698eb4ddb5658712a980f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039529"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="2a860-106">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a860-106">roleAssignment resource type</span></span>

<span data-ttu-id="2a860-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a860-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a860-108">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a860-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a860-109">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a860-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a860-110">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="2a860-110">The Role Assignment resource.</span></span> <span data-ttu-id="2a860-111">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="2a860-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="2a860-112">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="2a860-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="2a860-113">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="2a860-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="2a860-114">方法</span><span class="sxs-lookup"><span data-stu-id="2a860-114">Methods</span></span>
|<span data-ttu-id="2a860-115">方法</span><span class="sxs-lookup"><span data-stu-id="2a860-115">Method</span></span>|<span data-ttu-id="2a860-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a860-116">Return Type</span></span>|<span data-ttu-id="2a860-117">说明</span><span class="sxs-lookup"><span data-stu-id="2a860-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a860-118">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2a860-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="2a860-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a860-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2a860-120">列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a860-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="2a860-121">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="2a860-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2a860-123">读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a860-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2a860-124">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="2a860-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2a860-126">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a860-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2a860-127">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="2a860-128">无</span><span class="sxs-lookup"><span data-stu-id="2a860-128">None</span></span>|<span data-ttu-id="2a860-129">删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="2a860-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="2a860-130">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="2a860-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2a860-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2a860-132">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a860-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a860-133">属性</span><span class="sxs-lookup"><span data-stu-id="2a860-133">Properties</span></span>
|<span data-ttu-id="2a860-134">属性</span><span class="sxs-lookup"><span data-stu-id="2a860-134">Property</span></span>|<span data-ttu-id="2a860-135">类型</span><span class="sxs-lookup"><span data-stu-id="2a860-135">Type</span></span>|<span data-ttu-id="2a860-136">说明</span><span class="sxs-lookup"><span data-stu-id="2a860-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a860-137">id</span><span class="sxs-lookup"><span data-stu-id="2a860-137">id</span></span>|<span data-ttu-id="2a860-138">String</span><span class="sxs-lookup"><span data-stu-id="2a860-138">String</span></span>|<span data-ttu-id="2a860-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a860-139">Key of the entity.</span></span> <span data-ttu-id="2a860-140">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="2a860-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2a860-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2a860-141">displayName</span></span>|<span data-ttu-id="2a860-142">String</span><span class="sxs-lookup"><span data-stu-id="2a860-142">String</span></span>|<span data-ttu-id="2a860-143">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="2a860-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="2a860-144">description</span><span class="sxs-lookup"><span data-stu-id="2a860-144">description</span></span>|<span data-ttu-id="2a860-145">String</span><span class="sxs-lookup"><span data-stu-id="2a860-145">String</span></span>|<span data-ttu-id="2a860-146">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="2a860-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="2a860-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="2a860-147">scopeMembers</span></span>|<span data-ttu-id="2a860-148">String collection</span><span class="sxs-lookup"><span data-stu-id="2a860-148">String collection</span></span>|<span data-ttu-id="2a860-149">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="2a860-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2a860-150">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="2a860-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="2a860-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="2a860-151">scopeType</span></span>|[<span data-ttu-id="2a860-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="2a860-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="2a860-153">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="2a860-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="2a860-154">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="2a860-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="2a860-155">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers"，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="2a860-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="2a860-156">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="2a860-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="2a860-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="2a860-157">resourceScopes</span></span>|<span data-ttu-id="2a860-158">String collection</span><span class="sxs-lookup"><span data-stu-id="2a860-158">String collection</span></span>|<span data-ttu-id="2a860-159">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="2a860-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2a860-160">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="2a860-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a860-161">关系</span><span class="sxs-lookup"><span data-stu-id="2a860-161">Relationships</span></span>
|<span data-ttu-id="2a860-162">关系</span><span class="sxs-lookup"><span data-stu-id="2a860-162">Relationship</span></span>|<span data-ttu-id="2a860-163">类型</span><span class="sxs-lookup"><span data-stu-id="2a860-163">Type</span></span>|<span data-ttu-id="2a860-164">说明</span><span class="sxs-lookup"><span data-stu-id="2a860-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a860-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2a860-165">roleDefinition</span></span>|[<span data-ttu-id="2a860-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2a860-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="2a860-167">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="2a860-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a860-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a860-168">JSON Representation</span></span>
<span data-ttu-id="2a860-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a860-169">Here is a JSON representation of the resource.</span></span>
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







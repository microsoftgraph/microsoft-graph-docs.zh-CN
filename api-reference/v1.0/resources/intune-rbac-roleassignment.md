---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8506b87975b69f90cf561e776e557bb472f1ffd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846149"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="68a23-106">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="68a23-106">roleAssignment resource type</span></span>

> <span data-ttu-id="68a23-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68a23-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68a23-108">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="68a23-108">The Role Assignment resource.</span></span> <span data-ttu-id="68a23-109">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="68a23-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="68a23-110">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="68a23-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="68a23-111">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="68a23-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="68a23-112">方法</span><span class="sxs-lookup"><span data-stu-id="68a23-112">Methods</span></span>
|<span data-ttu-id="68a23-113">方法</span><span class="sxs-lookup"><span data-stu-id="68a23-113">Method</span></span>|<span data-ttu-id="68a23-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="68a23-114">Return Type</span></span>|<span data-ttu-id="68a23-115">说明</span><span class="sxs-lookup"><span data-stu-id="68a23-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68a23-116">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="68a23-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="68a23-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68a23-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="68a23-118">列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68a23-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="68a23-119">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="68a23-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="68a23-121">读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68a23-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="68a23-122">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="68a23-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="68a23-124">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68a23-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="68a23-125">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="68a23-126">无</span><span class="sxs-lookup"><span data-stu-id="68a23-126">None</span></span>|<span data-ttu-id="68a23-127">删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="68a23-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="68a23-128">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="68a23-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="68a23-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="68a23-130">更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68a23-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68a23-131">属性</span><span class="sxs-lookup"><span data-stu-id="68a23-131">Properties</span></span>
|<span data-ttu-id="68a23-132">属性</span><span class="sxs-lookup"><span data-stu-id="68a23-132">Property</span></span>|<span data-ttu-id="68a23-133">类型</span><span class="sxs-lookup"><span data-stu-id="68a23-133">Type</span></span>|<span data-ttu-id="68a23-134">说明</span><span class="sxs-lookup"><span data-stu-id="68a23-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a23-135">id</span><span class="sxs-lookup"><span data-stu-id="68a23-135">id</span></span>|<span data-ttu-id="68a23-136">String</span><span class="sxs-lookup"><span data-stu-id="68a23-136">String</span></span>|<span data-ttu-id="68a23-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="68a23-137">Key of the entity.</span></span> <span data-ttu-id="68a23-138">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="68a23-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="68a23-139">displayName</span><span class="sxs-lookup"><span data-stu-id="68a23-139">displayName</span></span>|<span data-ttu-id="68a23-140">String</span><span class="sxs-lookup"><span data-stu-id="68a23-140">String</span></span>|<span data-ttu-id="68a23-141">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="68a23-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="68a23-142">description</span><span class="sxs-lookup"><span data-stu-id="68a23-142">description</span></span>|<span data-ttu-id="68a23-143">String</span><span class="sxs-lookup"><span data-stu-id="68a23-143">String</span></span>|<span data-ttu-id="68a23-144">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="68a23-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="68a23-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="68a23-145">resourceScopes</span></span>|<span data-ttu-id="68a23-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="68a23-146">String collection</span></span>|<span data-ttu-id="68a23-147">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="68a23-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="68a23-148">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="68a23-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68a23-149">关系</span><span class="sxs-lookup"><span data-stu-id="68a23-149">Relationships</span></span>
|<span data-ttu-id="68a23-150">关系</span><span class="sxs-lookup"><span data-stu-id="68a23-150">Relationship</span></span>|<span data-ttu-id="68a23-151">类型</span><span class="sxs-lookup"><span data-stu-id="68a23-151">Type</span></span>|<span data-ttu-id="68a23-152">说明</span><span class="sxs-lookup"><span data-stu-id="68a23-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a23-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="68a23-153">roleDefinition</span></span>|[<span data-ttu-id="68a23-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="68a23-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="68a23-155">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="68a23-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68a23-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68a23-156">JSON Representation</span></span>
<span data-ttu-id="68a23-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68a23-157">Here is a JSON representation of the resource.</span></span>
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




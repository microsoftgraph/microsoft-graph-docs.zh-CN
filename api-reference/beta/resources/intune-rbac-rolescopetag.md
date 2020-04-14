---
title: roleScopeTag 资源类型
description: 角色范围标记
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9b30b3944976b2d8d0ac13aeb658402849c0b2d6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356815"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="0fca6-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fca6-103">roleScopeTag resource type</span></span>

<span data-ttu-id="0fca6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fca6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fca6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fca6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fca6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fca6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fca6-107">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="0fca6-107">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="0fca6-108">方法</span><span class="sxs-lookup"><span data-stu-id="0fca6-108">Methods</span></span>
|<span data-ttu-id="0fca6-109">方法</span><span class="sxs-lookup"><span data-stu-id="0fca6-109">Method</span></span>|<span data-ttu-id="0fca6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fca6-110">Return Type</span></span>|<span data-ttu-id="0fca6-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fca6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fca6-112">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fca6-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="0fca6-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fca6-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0fca6-114">列出[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fca6-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="0fca6-115">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="0fca6-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0fca6-117">读取[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fca6-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0fca6-118">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="0fca6-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0fca6-120">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0fca6-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0fca6-121">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="0fca6-122">无</span><span class="sxs-lookup"><span data-stu-id="0fca6-122">None</span></span>|<span data-ttu-id="0fca6-123">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="0fca6-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="0fca6-124">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="0fca6-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0fca6-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0fca6-126">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fca6-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0fca6-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="0fca6-127">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="0fca6-128">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fca6-128">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="0fca6-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fca6-129">Not yet documented</span></span>|
|[<span data-ttu-id="0fca6-130">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="0fca6-130">getRoleScopeTagsById action</span></span>](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|<span data-ttu-id="0fca6-131">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fca6-131">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0fca6-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fca6-132">Not yet documented</span></span>|
|[<span data-ttu-id="0fca6-133">hasCustomRoleScopeTag 函数</span><span class="sxs-lookup"><span data-stu-id="0fca6-133">hasCustomRoleScopeTag function</span></span>](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|<span data-ttu-id="0fca6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fca6-134">Boolean</span></span>|<span data-ttu-id="0fca6-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fca6-135">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0fca6-136">属性</span><span class="sxs-lookup"><span data-stu-id="0fca6-136">Properties</span></span>
|<span data-ttu-id="0fca6-137">属性</span><span class="sxs-lookup"><span data-stu-id="0fca6-137">Property</span></span>|<span data-ttu-id="0fca6-138">类型</span><span class="sxs-lookup"><span data-stu-id="0fca6-138">Type</span></span>|<span data-ttu-id="0fca6-139">说明</span><span class="sxs-lookup"><span data-stu-id="0fca6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fca6-140">id</span><span class="sxs-lookup"><span data-stu-id="0fca6-140">id</span></span>|<span data-ttu-id="0fca6-141">字符串</span><span class="sxs-lookup"><span data-stu-id="0fca6-141">String</span></span>|<span data-ttu-id="0fca6-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fca6-142">Key of the entity.</span></span> <span data-ttu-id="0fca6-143">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="0fca6-143">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0fca6-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0fca6-144">displayName</span></span>|<span data-ttu-id="0fca6-145">String</span><span class="sxs-lookup"><span data-stu-id="0fca6-145">String</span></span>|<span data-ttu-id="0fca6-146">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="0fca6-146">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0fca6-147">description</span><span class="sxs-lookup"><span data-stu-id="0fca6-147">description</span></span>|<span data-ttu-id="0fca6-148">String</span><span class="sxs-lookup"><span data-stu-id="0fca6-148">String</span></span>|<span data-ttu-id="0fca6-149">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="0fca6-149">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0fca6-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0fca6-150">isBuiltIn</span></span>|<span data-ttu-id="0fca6-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fca6-151">Boolean</span></span>|<span data-ttu-id="0fca6-152">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="0fca6-152">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fca6-153">关系</span><span class="sxs-lookup"><span data-stu-id="0fca6-153">Relationships</span></span>
|<span data-ttu-id="0fca6-154">关系</span><span class="sxs-lookup"><span data-stu-id="0fca6-154">Relationship</span></span>|<span data-ttu-id="0fca6-155">类型</span><span class="sxs-lookup"><span data-stu-id="0fca6-155">Type</span></span>|<span data-ttu-id="0fca6-156">说明</span><span class="sxs-lookup"><span data-stu-id="0fca6-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fca6-157">assignments</span><span class="sxs-lookup"><span data-stu-id="0fca6-157">assignments</span></span>|<span data-ttu-id="0fca6-158">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fca6-158">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="0fca6-159">此角色作用域标记的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0fca6-159">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fca6-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fca6-160">JSON Representation</span></span>
<span data-ttu-id="0fca6-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fca6-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": true
}
```




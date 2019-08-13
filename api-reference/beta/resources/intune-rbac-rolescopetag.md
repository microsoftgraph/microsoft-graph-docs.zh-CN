---
title: roleScopeTag 资源类型
description: 角色范围标记
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4eff14cb14bc9edd1a676eeeb543a599c2d032b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369197"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="9b76f-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b76f-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="9b76f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b76f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b76f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b76f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b76f-106">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="9b76f-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="9b76f-107">方法</span><span class="sxs-lookup"><span data-stu-id="9b76f-107">Methods</span></span>
|<span data-ttu-id="9b76f-108">方法</span><span class="sxs-lookup"><span data-stu-id="9b76f-108">Method</span></span>|<span data-ttu-id="9b76f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9b76f-109">Return Type</span></span>|<span data-ttu-id="9b76f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b76f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b76f-111">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b76f-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="9b76f-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b76f-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="9b76f-113">列出[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b76f-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="9b76f-114">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="9b76f-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9b76f-116">读取[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b76f-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="9b76f-117">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="9b76f-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9b76f-119">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b76f-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="9b76f-120">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="9b76f-121">无</span><span class="sxs-lookup"><span data-stu-id="9b76f-121">None</span></span>|<span data-ttu-id="9b76f-122">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="9b76f-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="9b76f-123">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="9b76f-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9b76f-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9b76f-125">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b76f-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="9b76f-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="9b76f-126">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="9b76f-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b76f-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="9b76f-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b76f-128">Not yet documented</span></span>|
|[<span data-ttu-id="9b76f-129">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="9b76f-129">getRoleScopeTagsById action</span></span>](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|<span data-ttu-id="9b76f-130">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b76f-130">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="9b76f-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b76f-131">Not yet documented</span></span>|
|[<span data-ttu-id="9b76f-132">hasCustomRoleScopeTag 函数</span><span class="sxs-lookup"><span data-stu-id="9b76f-132">hasCustomRoleScopeTag function</span></span>](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|<span data-ttu-id="9b76f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b76f-133">Boolean</span></span>|<span data-ttu-id="9b76f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b76f-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9b76f-135">属性</span><span class="sxs-lookup"><span data-stu-id="9b76f-135">Properties</span></span>
|<span data-ttu-id="9b76f-136">属性</span><span class="sxs-lookup"><span data-stu-id="9b76f-136">Property</span></span>|<span data-ttu-id="9b76f-137">类型</span><span class="sxs-lookup"><span data-stu-id="9b76f-137">Type</span></span>|<span data-ttu-id="9b76f-138">说明</span><span class="sxs-lookup"><span data-stu-id="9b76f-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b76f-139">id</span><span class="sxs-lookup"><span data-stu-id="9b76f-139">id</span></span>|<span data-ttu-id="9b76f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9b76f-140">String</span></span>|<span data-ttu-id="9b76f-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b76f-141">Key of the entity.</span></span> <span data-ttu-id="9b76f-142">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="9b76f-142">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9b76f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="9b76f-143">displayName</span></span>|<span data-ttu-id="9b76f-144">String</span><span class="sxs-lookup"><span data-stu-id="9b76f-144">String</span></span>|<span data-ttu-id="9b76f-145">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="9b76f-145">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="9b76f-146">说明</span><span class="sxs-lookup"><span data-stu-id="9b76f-146">description</span></span>|<span data-ttu-id="9b76f-147">String</span><span class="sxs-lookup"><span data-stu-id="9b76f-147">String</span></span>|<span data-ttu-id="9b76f-148">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="9b76f-148">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="9b76f-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9b76f-149">isBuiltIn</span></span>|<span data-ttu-id="9b76f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b76f-150">Boolean</span></span>|<span data-ttu-id="9b76f-151">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="9b76f-151">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b76f-152">关系</span><span class="sxs-lookup"><span data-stu-id="9b76f-152">Relationships</span></span>
|<span data-ttu-id="9b76f-153">关系</span><span class="sxs-lookup"><span data-stu-id="9b76f-153">Relationship</span></span>|<span data-ttu-id="9b76f-154">类型</span><span class="sxs-lookup"><span data-stu-id="9b76f-154">Type</span></span>|<span data-ttu-id="9b76f-155">说明</span><span class="sxs-lookup"><span data-stu-id="9b76f-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b76f-156">assignments</span><span class="sxs-lookup"><span data-stu-id="9b76f-156">assignments</span></span>|<span data-ttu-id="9b76f-157">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b76f-157">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="9b76f-158">此角色作用域标记的分配列表。</span><span class="sxs-lookup"><span data-stu-id="9b76f-158">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b76f-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b76f-159">JSON Representation</span></span>
<span data-ttu-id="9b76f-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b76f-160">Here is a JSON representation of the resource.</span></span>
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




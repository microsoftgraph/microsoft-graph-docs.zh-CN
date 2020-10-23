---
title: roleScopeTag 资源类型
description: 角色范围标记
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff18fcc1ee8575d760cf748f0c75f147d31b9d92
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697208"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="f4383-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4383-103">roleScopeTag resource type</span></span>

<span data-ttu-id="f4383-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4383-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4383-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4383-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4383-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4383-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4383-107">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="f4383-107">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="f4383-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f4383-108">Methods</span></span>
|<span data-ttu-id="f4383-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4383-109">Method</span></span>|<span data-ttu-id="f4383-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4383-110">Return Type</span></span>|<span data-ttu-id="f4383-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4383-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4383-112">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4383-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="f4383-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4383-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="f4383-114">列出 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4383-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="f4383-115">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="f4383-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="f4383-117">读取 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4383-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="f4383-118">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="f4383-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="f4383-120">创建新的 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4383-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="f4383-121">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="f4383-122">无</span><span class="sxs-lookup"><span data-stu-id="f4383-122">None</span></span>|<span data-ttu-id="f4383-123">删除 [roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="f4383-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="f4383-124">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="f4383-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f4383-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="f4383-126">更新 [roleScopeTag](../resources/intune-rbac-rolescopetag.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4383-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="f4383-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="f4383-127">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="f4383-128">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4383-128">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="f4383-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4383-129">Not yet documented</span></span>|
|[<span data-ttu-id="f4383-130">getRoleScopeTagsById 操作</span><span class="sxs-lookup"><span data-stu-id="f4383-130">getRoleScopeTagsById action</span></span>](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|<span data-ttu-id="f4383-131">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4383-131">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="f4383-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4383-132">Not yet documented</span></span>|
|[<span data-ttu-id="f4383-133">hasCustomRoleScopeTag 函数</span><span class="sxs-lookup"><span data-stu-id="f4383-133">hasCustomRoleScopeTag function</span></span>](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|<span data-ttu-id="f4383-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4383-134">Boolean</span></span>|<span data-ttu-id="f4383-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4383-135">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f4383-136">属性</span><span class="sxs-lookup"><span data-stu-id="f4383-136">Properties</span></span>
|<span data-ttu-id="f4383-137">属性</span><span class="sxs-lookup"><span data-stu-id="f4383-137">Property</span></span>|<span data-ttu-id="f4383-138">类型</span><span class="sxs-lookup"><span data-stu-id="f4383-138">Type</span></span>|<span data-ttu-id="f4383-139">说明</span><span class="sxs-lookup"><span data-stu-id="f4383-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4383-140">id</span><span class="sxs-lookup"><span data-stu-id="f4383-140">id</span></span>|<span data-ttu-id="f4383-141">String</span><span class="sxs-lookup"><span data-stu-id="f4383-141">String</span></span>|<span data-ttu-id="f4383-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4383-142">Key of the entity.</span></span> <span data-ttu-id="f4383-143">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="f4383-143">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f4383-144">displayName</span><span class="sxs-lookup"><span data-stu-id="f4383-144">displayName</span></span>|<span data-ttu-id="f4383-145">String</span><span class="sxs-lookup"><span data-stu-id="f4383-145">String</span></span>|<span data-ttu-id="f4383-146">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="f4383-146">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f4383-147">说明</span><span class="sxs-lookup"><span data-stu-id="f4383-147">description</span></span>|<span data-ttu-id="f4383-148">String</span><span class="sxs-lookup"><span data-stu-id="f4383-148">String</span></span>|<span data-ttu-id="f4383-149">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="f4383-149">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f4383-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f4383-150">isBuiltIn</span></span>|<span data-ttu-id="f4383-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4383-151">Boolean</span></span>|<span data-ttu-id="f4383-152">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="f4383-152">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4383-153">关系</span><span class="sxs-lookup"><span data-stu-id="f4383-153">Relationships</span></span>
|<span data-ttu-id="f4383-154">关系</span><span class="sxs-lookup"><span data-stu-id="f4383-154">Relationship</span></span>|<span data-ttu-id="f4383-155">类型</span><span class="sxs-lookup"><span data-stu-id="f4383-155">Type</span></span>|<span data-ttu-id="f4383-156">说明</span><span class="sxs-lookup"><span data-stu-id="f4383-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4383-157">assignments</span><span class="sxs-lookup"><span data-stu-id="f4383-157">assignments</span></span>|<span data-ttu-id="f4383-158">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4383-158">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="f4383-159">此角色作用域标记的分配列表。</span><span class="sxs-lookup"><span data-stu-id="f4383-159">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4383-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4383-160">JSON Representation</span></span>
<span data-ttu-id="f4383-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4383-161">Here is a JSON representation of the resource.</span></span>
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






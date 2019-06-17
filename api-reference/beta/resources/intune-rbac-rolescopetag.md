---
title: roleScopeTag 资源类型
description: 角色范围标记
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54aa59e99a9697924512da0072e7b4e05e4fa12a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993534"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="5363e-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="5363e-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="5363e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5363e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5363e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5363e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5363e-106">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="5363e-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="5363e-107">方法</span><span class="sxs-lookup"><span data-stu-id="5363e-107">Methods</span></span>
|<span data-ttu-id="5363e-108">方法</span><span class="sxs-lookup"><span data-stu-id="5363e-108">Method</span></span>|<span data-ttu-id="5363e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5363e-109">Return Type</span></span>|<span data-ttu-id="5363e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5363e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5363e-111">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="5363e-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="5363e-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="5363e-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="5363e-113">列出[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5363e-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="5363e-114">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="5363e-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="5363e-116">读取[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5363e-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="5363e-117">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="5363e-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="5363e-119">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5363e-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="5363e-120">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="5363e-121">无</span><span class="sxs-lookup"><span data-stu-id="5363e-121">None</span></span>|<span data-ttu-id="5363e-122">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="5363e-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="5363e-123">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="5363e-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5363e-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="5363e-125">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5363e-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="5363e-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="5363e-126">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="5363e-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5363e-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="5363e-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5363e-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5363e-129">属性</span><span class="sxs-lookup"><span data-stu-id="5363e-129">Properties</span></span>
|<span data-ttu-id="5363e-130">属性</span><span class="sxs-lookup"><span data-stu-id="5363e-130">Property</span></span>|<span data-ttu-id="5363e-131">类型</span><span class="sxs-lookup"><span data-stu-id="5363e-131">Type</span></span>|<span data-ttu-id="5363e-132">说明</span><span class="sxs-lookup"><span data-stu-id="5363e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5363e-133">id</span><span class="sxs-lookup"><span data-stu-id="5363e-133">id</span></span>|<span data-ttu-id="5363e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5363e-134">String</span></span>|<span data-ttu-id="5363e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5363e-135">Key of the entity.</span></span> <span data-ttu-id="5363e-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="5363e-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5363e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5363e-137">displayName</span></span>|<span data-ttu-id="5363e-138">String</span><span class="sxs-lookup"><span data-stu-id="5363e-138">String</span></span>|<span data-ttu-id="5363e-139">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="5363e-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="5363e-140">说明</span><span class="sxs-lookup"><span data-stu-id="5363e-140">description</span></span>|<span data-ttu-id="5363e-141">String</span><span class="sxs-lookup"><span data-stu-id="5363e-141">String</span></span>|<span data-ttu-id="5363e-142">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="5363e-142">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5363e-143">关系</span><span class="sxs-lookup"><span data-stu-id="5363e-143">Relationships</span></span>
|<span data-ttu-id="5363e-144">关系</span><span class="sxs-lookup"><span data-stu-id="5363e-144">Relationship</span></span>|<span data-ttu-id="5363e-145">类型</span><span class="sxs-lookup"><span data-stu-id="5363e-145">Type</span></span>|<span data-ttu-id="5363e-146">说明</span><span class="sxs-lookup"><span data-stu-id="5363e-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5363e-147">assignments</span><span class="sxs-lookup"><span data-stu-id="5363e-147">assignments</span></span>|<span data-ttu-id="5363e-148">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5363e-148">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="5363e-149">此角色作用域标记的分配列表。</span><span class="sxs-lookup"><span data-stu-id="5363e-149">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5363e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5363e-150">JSON Representation</span></span>
<span data-ttu-id="5363e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5363e-151">Here is a JSON representation of the resource.</span></span>
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
  "description": "String"
}
```






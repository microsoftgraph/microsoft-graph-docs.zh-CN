---
title: roleScopeTag 资源类型
description: 角色范围标记
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6916521c8edef1b1decfb6b006779a372d3ab4e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566323"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="d57b9-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="d57b9-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="d57b9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d57b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d57b9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d57b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57b9-106">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="d57b9-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="d57b9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d57b9-107">Methods</span></span>
|<span data-ttu-id="d57b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="d57b9-108">Method</span></span>|<span data-ttu-id="d57b9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d57b9-109">Return Type</span></span>|<span data-ttu-id="d57b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="d57b9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d57b9-111">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="d57b9-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="d57b9-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="d57b9-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="d57b9-113">列出[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d57b9-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="d57b9-114">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="d57b9-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="d57b9-116">读取[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d57b9-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="d57b9-117">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="d57b9-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="d57b9-119">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d57b9-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="d57b9-120">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="d57b9-121">无</span><span class="sxs-lookup"><span data-stu-id="d57b9-121">None</span></span>|<span data-ttu-id="d57b9-122">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="d57b9-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="d57b9-123">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="d57b9-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d57b9-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="d57b9-125">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d57b9-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d57b9-126">属性</span><span class="sxs-lookup"><span data-stu-id="d57b9-126">Properties</span></span>
|<span data-ttu-id="d57b9-127">属性</span><span class="sxs-lookup"><span data-stu-id="d57b9-127">Property</span></span>|<span data-ttu-id="d57b9-128">类型</span><span class="sxs-lookup"><span data-stu-id="d57b9-128">Type</span></span>|<span data-ttu-id="d57b9-129">说明</span><span class="sxs-lookup"><span data-stu-id="d57b9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57b9-130">id</span><span class="sxs-lookup"><span data-stu-id="d57b9-130">id</span></span>|<span data-ttu-id="d57b9-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d57b9-131">String</span></span>|<span data-ttu-id="d57b9-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d57b9-132">Key of the entity.</span></span> <span data-ttu-id="d57b9-133">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="d57b9-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d57b9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d57b9-134">displayName</span></span>|<span data-ttu-id="d57b9-135">String</span><span class="sxs-lookup"><span data-stu-id="d57b9-135">String</span></span>|<span data-ttu-id="d57b9-136">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="d57b9-136">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="d57b9-137">说明</span><span class="sxs-lookup"><span data-stu-id="d57b9-137">description</span></span>|<span data-ttu-id="d57b9-138">String</span><span class="sxs-lookup"><span data-stu-id="d57b9-138">String</span></span>|<span data-ttu-id="d57b9-139">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="d57b9-139">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d57b9-140">关系</span><span class="sxs-lookup"><span data-stu-id="d57b9-140">Relationships</span></span>
<span data-ttu-id="d57b9-141">无</span><span class="sxs-lookup"><span data-stu-id="d57b9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d57b9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d57b9-142">JSON Representation</span></span>
<span data-ttu-id="d57b9-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d57b9-143">Here is a JSON representation of the resource.</span></span>
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






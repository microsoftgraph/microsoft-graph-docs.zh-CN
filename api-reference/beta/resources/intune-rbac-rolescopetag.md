---
title: roleScopeTag 资源类型
description: 角色范围标记
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c7bfb12172f6ae99f14a65647a7a6ab8955fef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159421"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="a7139-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7139-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="a7139-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7139-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7139-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7139-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7139-106">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="a7139-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="a7139-107">方法</span><span class="sxs-lookup"><span data-stu-id="a7139-107">Methods</span></span>
|<span data-ttu-id="a7139-108">方法</span><span class="sxs-lookup"><span data-stu-id="a7139-108">Method</span></span>|<span data-ttu-id="a7139-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7139-109">Return Type</span></span>|<span data-ttu-id="a7139-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7139-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7139-111">列出 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7139-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="a7139-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="a7139-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="a7139-113">列出[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7139-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="a7139-114">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="a7139-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a7139-116">读取[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7139-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="a7139-117">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="a7139-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a7139-119">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7139-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="a7139-120">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="a7139-121">无</span><span class="sxs-lookup"><span data-stu-id="a7139-121">None</span></span>|<span data-ttu-id="a7139-122">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="a7139-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="a7139-123">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="a7139-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a7139-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a7139-125">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7139-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7139-126">属性</span><span class="sxs-lookup"><span data-stu-id="a7139-126">Properties</span></span>
|<span data-ttu-id="a7139-127">属性</span><span class="sxs-lookup"><span data-stu-id="a7139-127">Property</span></span>|<span data-ttu-id="a7139-128">类型</span><span class="sxs-lookup"><span data-stu-id="a7139-128">Type</span></span>|<span data-ttu-id="a7139-129">说明</span><span class="sxs-lookup"><span data-stu-id="a7139-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7139-130">id</span><span class="sxs-lookup"><span data-stu-id="a7139-130">id</span></span>|<span data-ttu-id="a7139-131">String</span><span class="sxs-lookup"><span data-stu-id="a7139-131">String</span></span>|<span data-ttu-id="a7139-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7139-132">Key of the entity.</span></span> <span data-ttu-id="a7139-133">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a7139-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a7139-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a7139-134">displayName</span></span>|<span data-ttu-id="a7139-135">字符串</span><span class="sxs-lookup"><span data-stu-id="a7139-135">String</span></span>|<span data-ttu-id="a7139-136">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a7139-136">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="a7139-137">说明</span><span class="sxs-lookup"><span data-stu-id="a7139-137">description</span></span>|<span data-ttu-id="a7139-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a7139-138">String</span></span>|<span data-ttu-id="a7139-139">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="a7139-139">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7139-140">关系</span><span class="sxs-lookup"><span data-stu-id="a7139-140">Relationships</span></span>
<span data-ttu-id="a7139-141">无</span><span class="sxs-lookup"><span data-stu-id="a7139-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7139-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7139-142">JSON Representation</span></span>
<span data-ttu-id="a7139-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7139-143">Here is a JSON representation of the resource.</span></span>
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





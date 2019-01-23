---
title: roleScopeTag 资源类型
description: 角色作用域标记
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400562"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="2b7c3-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b7c3-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="2b7c3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b7c3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b7c3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7c3-107">角色作用域标记</span><span class="sxs-lookup"><span data-stu-id="2b7c3-107">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="2b7c3-108">方法</span><span class="sxs-lookup"><span data-stu-id="2b7c3-108">Methods</span></span>
|<span data-ttu-id="2b7c3-109">方法</span><span class="sxs-lookup"><span data-stu-id="2b7c3-109">Method</span></span>|<span data-ttu-id="2b7c3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b7c3-110">Return Type</span></span>|<span data-ttu-id="2b7c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b7c3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b7c3-112">列表 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b7c3-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="2b7c3-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b7c3-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="2b7c3-114">列出属性和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="2b7c3-115">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="2b7c3-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="2b7c3-117">读取属性和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="2b7c3-118">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="2b7c3-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="2b7c3-120">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="2b7c3-121">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="2b7c3-122">无</span><span class="sxs-lookup"><span data-stu-id="2b7c3-122">None</span></span>|<span data-ttu-id="2b7c3-123">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="2b7c3-124">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="2b7c3-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b7c3-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="2b7c3-126">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b7c3-127">属性</span><span class="sxs-lookup"><span data-stu-id="2b7c3-127">Properties</span></span>
|<span data-ttu-id="2b7c3-128">属性</span><span class="sxs-lookup"><span data-stu-id="2b7c3-128">Property</span></span>|<span data-ttu-id="2b7c3-129">类型</span><span class="sxs-lookup"><span data-stu-id="2b7c3-129">Type</span></span>|<span data-ttu-id="2b7c3-130">说明</span><span class="sxs-lookup"><span data-stu-id="2b7c3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7c3-131">id</span><span class="sxs-lookup"><span data-stu-id="2b7c3-131">id</span></span>|<span data-ttu-id="2b7c3-132">String</span><span class="sxs-lookup"><span data-stu-id="2b7c3-132">String</span></span>|<span data-ttu-id="2b7c3-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-133">Key of the entity.</span></span> <span data-ttu-id="2b7c3-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2b7c3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7c3-135">displayName</span></span>|<span data-ttu-id="2b7c3-136">String</span><span class="sxs-lookup"><span data-stu-id="2b7c3-136">String</span></span>|<span data-ttu-id="2b7c3-137">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="2b7c3-138">说明</span><span class="sxs-lookup"><span data-stu-id="2b7c3-138">description</span></span>|<span data-ttu-id="2b7c3-139">String</span><span class="sxs-lookup"><span data-stu-id="2b7c3-139">String</span></span>|<span data-ttu-id="2b7c3-140">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b7c3-141">关系</span><span class="sxs-lookup"><span data-stu-id="2b7c3-141">Relationships</span></span>
<span data-ttu-id="2b7c3-142">无</span><span class="sxs-lookup"><span data-stu-id="2b7c3-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b7c3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b7c3-143">JSON Representation</span></span>
<span data-ttu-id="2b7c3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b7c3-144">Here is a JSON representation of the resource.</span></span>
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





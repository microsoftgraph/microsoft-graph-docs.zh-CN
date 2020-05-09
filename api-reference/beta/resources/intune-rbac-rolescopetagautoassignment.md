---
title: roleScopeTagAutoAssignment 资源类型
description: 包含用于将角色作用域标记自动分配给要应用于设备的组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df95dff1efb35e6f8ac7d20ec99c83f89222786b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177287"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="48ad5-103">roleScopeTagAutoAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="48ad5-103">roleScopeTagAutoAssignment resource type</span></span>

<span data-ttu-id="48ad5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48ad5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48ad5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="48ad5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48ad5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48ad5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48ad5-107">包含用于将角色作用域标记自动分配给要应用于设备的组的属性。</span><span class="sxs-lookup"><span data-stu-id="48ad5-107">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="48ad5-108">方法</span><span class="sxs-lookup"><span data-stu-id="48ad5-108">Methods</span></span>
|<span data-ttu-id="48ad5-109">方法</span><span class="sxs-lookup"><span data-stu-id="48ad5-109">Method</span></span>|<span data-ttu-id="48ad5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="48ad5-110">Return Type</span></span>|<span data-ttu-id="48ad5-111">说明</span><span class="sxs-lookup"><span data-stu-id="48ad5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48ad5-112">列出 roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="48ad5-112">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="48ad5-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="48ad5-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="48ad5-114">列出[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48ad5-114">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="48ad5-115">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-115">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="48ad5-116">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-116">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="48ad5-117">读取[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48ad5-117">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="48ad5-118">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-118">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="48ad5-119">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-119">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="48ad5-120">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48ad5-120">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="48ad5-121">删除 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-121">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="48ad5-122">无</span><span class="sxs-lookup"><span data-stu-id="48ad5-122">None</span></span>|<span data-ttu-id="48ad5-123">删除[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="48ad5-123">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="48ad5-124">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-124">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="48ad5-125">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="48ad5-125">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="48ad5-126">更新[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48ad5-126">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="48ad5-127">属性</span><span class="sxs-lookup"><span data-stu-id="48ad5-127">Properties</span></span>
|<span data-ttu-id="48ad5-128">属性</span><span class="sxs-lookup"><span data-stu-id="48ad5-128">Property</span></span>|<span data-ttu-id="48ad5-129">类型</span><span class="sxs-lookup"><span data-stu-id="48ad5-129">Type</span></span>|<span data-ttu-id="48ad5-130">说明</span><span class="sxs-lookup"><span data-stu-id="48ad5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48ad5-131">id</span><span class="sxs-lookup"><span data-stu-id="48ad5-131">id</span></span>|<span data-ttu-id="48ad5-132">字符串</span><span class="sxs-lookup"><span data-stu-id="48ad5-132">String</span></span>|<span data-ttu-id="48ad5-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48ad5-133">Key of the entity.</span></span>|
|<span data-ttu-id="48ad5-134">target</span><span class="sxs-lookup"><span data-stu-id="48ad5-134">target</span></span>|[<span data-ttu-id="48ad5-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="48ad5-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="48ad5-136">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="48ad5-136">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48ad5-137">关系</span><span class="sxs-lookup"><span data-stu-id="48ad5-137">Relationships</span></span>
<span data-ttu-id="48ad5-138">无</span><span class="sxs-lookup"><span data-stu-id="48ad5-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48ad5-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48ad5-139">JSON Representation</span></span>
<span data-ttu-id="48ad5-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48ad5-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```




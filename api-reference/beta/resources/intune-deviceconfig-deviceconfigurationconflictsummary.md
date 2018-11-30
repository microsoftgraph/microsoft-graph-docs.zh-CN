---
title: deviceConfigurationConflictSummary 资源类型
description: 冲突一设备配置策略的摘要。
ms.openlocfilehash: b292dd40bfb0502aa55109072ee9e9f59a8eb45a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045322"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="b82bf-103">deviceConfigurationConflictSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b82bf-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="b82bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b82bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b82bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b82bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b82bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b82bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b82bf-107">冲突一设备配置策略的摘要。</span><span class="sxs-lookup"><span data-stu-id="b82bf-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="methods"></a><span data-ttu-id="b82bf-108">方法</span><span class="sxs-lookup"><span data-stu-id="b82bf-108">Methods</span></span>
|<span data-ttu-id="b82bf-109">方法</span><span class="sxs-lookup"><span data-stu-id="b82bf-109">Method</span></span>|<span data-ttu-id="b82bf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b82bf-110">Return Type</span></span>|<span data-ttu-id="b82bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="b82bf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b82bf-112">列表 deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="b82bf-112">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="b82bf-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="b82bf-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="b82bf-114">列出属性和[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="b82bf-114">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="b82bf-115">获取 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-115">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="b82bf-116">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-116">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="b82bf-117">读取属性和[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="b82bf-117">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="b82bf-118">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-118">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="b82bf-119">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-119">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="b82bf-120">创建新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b82bf-120">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="b82bf-121">删除 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-121">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="b82bf-122">无</span><span class="sxs-lookup"><span data-stu-id="b82bf-122">None</span></span>|<span data-ttu-id="b82bf-123">删除[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="b82bf-123">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="b82bf-124">更新 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-124">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="b82bf-125">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="b82bf-125">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="b82bf-126">更新[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b82bf-126">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b82bf-127">属性</span><span class="sxs-lookup"><span data-stu-id="b82bf-127">Properties</span></span>
|<span data-ttu-id="b82bf-128">属性</span><span class="sxs-lookup"><span data-stu-id="b82bf-128">Property</span></span>|<span data-ttu-id="b82bf-129">类型</span><span class="sxs-lookup"><span data-stu-id="b82bf-129">Type</span></span>|<span data-ttu-id="b82bf-130">说明</span><span class="sxs-lookup"><span data-stu-id="b82bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82bf-131">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="b82bf-131">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="b82bf-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b82bf-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b82bf-133">组策略的给定设置冲突</span><span class="sxs-lookup"><span data-stu-id="b82bf-133">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="b82bf-134">id</span><span class="sxs-lookup"><span data-stu-id="b82bf-134">id</span></span>|<span data-ttu-id="b82bf-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b82bf-135">String</span></span>|<span data-ttu-id="b82bf-136">冲突策略的这组 id。</span><span class="sxs-lookup"><span data-stu-id="b82bf-136">The id for this set of conflicting policies.</span></span> <span data-ttu-id="b82bf-137">此 id 是分隔下划线字典顺序 ConflictingDeviceConfigurations 中的所有策略的 id。</span><span class="sxs-lookup"><span data-stu-id="b82bf-137">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="b82bf-138">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="b82bf-138">contributingSettings</span></span>|<span data-ttu-id="b82bf-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="b82bf-139">String collection</span></span>|<span data-ttu-id="b82bf-140">冲突的给定的策略设置的集合</span><span class="sxs-lookup"><span data-stu-id="b82bf-140">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="b82bf-141">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="b82bf-141">deviceCheckinsImpacted</span></span>|<span data-ttu-id="b82bf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b82bf-142">Int32</span></span>|<span data-ttu-id="b82bf-143">签入受影响的冲突的策略和设置的计数</span><span class="sxs-lookup"><span data-stu-id="b82bf-143">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="b82bf-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="b82bf-144">Relationships</span></span>
<span data-ttu-id="b82bf-145">无</span><span class="sxs-lookup"><span data-stu-id="b82bf-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b82bf-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b82bf-146">JSON Representation</span></span>
<span data-ttu-id="b82bf-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b82bf-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```






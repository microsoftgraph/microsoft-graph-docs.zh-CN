---
title: deviceConfigurationConflictSummary 资源类型
description: 冲突一设备配置策略的摘要。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f8d84a4240059ff9772fefd9737ad27d8fbae7a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843335"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="5b5b1-103">deviceConfigurationConflictSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b5b1-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="5b5b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b5b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b5b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b5b1-107">冲突一设备配置策略的摘要。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="methods"></a><span data-ttu-id="5b5b1-108">方法</span><span class="sxs-lookup"><span data-stu-id="5b5b1-108">Methods</span></span>
|<span data-ttu-id="5b5b1-109">方法</span><span class="sxs-lookup"><span data-stu-id="5b5b1-109">Method</span></span>|<span data-ttu-id="5b5b1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b5b1-110">Return Type</span></span>|<span data-ttu-id="5b5b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b5b1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b5b1-112">列表 deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="5b5b1-112">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="5b5b1-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="5b5b1-113">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="5b5b1-114">列出属性和[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-114">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="5b5b1-115">获取 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-115">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="5b5b1-116">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-116">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="5b5b1-117">读取属性和[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-117">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="5b5b1-118">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-118">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="5b5b1-119">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-119">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="5b5b1-120">创建新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-120">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="5b5b1-121">删除 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-121">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="5b5b1-122">无</span><span class="sxs-lookup"><span data-stu-id="5b5b1-122">None</span></span>|<span data-ttu-id="5b5b1-123">删除[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-123">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="5b5b1-124">更新 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-124">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="5b5b1-125">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="5b5b1-125">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="5b5b1-126">更新[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-126">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b5b1-127">属性</span><span class="sxs-lookup"><span data-stu-id="5b5b1-127">Properties</span></span>
|<span data-ttu-id="5b5b1-128">属性</span><span class="sxs-lookup"><span data-stu-id="5b5b1-128">Property</span></span>|<span data-ttu-id="5b5b1-129">类型</span><span class="sxs-lookup"><span data-stu-id="5b5b1-129">Type</span></span>|<span data-ttu-id="5b5b1-130">Description</span><span class="sxs-lookup"><span data-stu-id="5b5b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5b1-131">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="5b5b1-131">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="5b5b1-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b5b1-132">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5b5b1-133">组策略的给定设置冲突</span><span class="sxs-lookup"><span data-stu-id="5b5b1-133">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="5b5b1-134">id</span><span class="sxs-lookup"><span data-stu-id="5b5b1-134">id</span></span>|<span data-ttu-id="5b5b1-135">字符串</span><span class="sxs-lookup"><span data-stu-id="5b5b1-135">String</span></span>|<span data-ttu-id="5b5b1-136">冲突策略的这组 id。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-136">The id for this set of conflicting policies.</span></span> <span data-ttu-id="5b5b1-137">此 id 是分隔下划线字典顺序 ConflictingDeviceConfigurations 中的所有策略的 id。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-137">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="5b5b1-138">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="5b5b1-138">contributingSettings</span></span>|<span data-ttu-id="5b5b1-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="5b5b1-139">String collection</span></span>|<span data-ttu-id="5b5b1-140">冲突的给定的策略设置的集合</span><span class="sxs-lookup"><span data-stu-id="5b5b1-140">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="5b5b1-141">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="5b5b1-141">deviceCheckinsImpacted</span></span>|<span data-ttu-id="5b5b1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5b5b1-142">Int32</span></span>|<span data-ttu-id="5b5b1-143">签入受影响的冲突的策略和设置的计数</span><span class="sxs-lookup"><span data-stu-id="5b5b1-143">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b5b1-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="5b5b1-144">Relationships</span></span>
<span data-ttu-id="5b5b1-145">无</span><span class="sxs-lookup"><span data-stu-id="5b5b1-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b5b1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b5b1-146">JSON Representation</span></span>
<span data-ttu-id="5b5b1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b5b1-147">Here is a JSON representation of the resource.</span></span>
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






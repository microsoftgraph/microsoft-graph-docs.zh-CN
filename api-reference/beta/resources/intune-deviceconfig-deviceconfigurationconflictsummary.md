---
title: deviceConfigurationConflictSummary 资源类型
description: 一组设备配置策略的冲突摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f4beeafbf6dd52cc29791bfde917e363c7077e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001654"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a><span data-ttu-id="31211-103">deviceConfigurationConflictSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="31211-103">deviceConfigurationConflictSummary resource type</span></span>

> <span data-ttu-id="31211-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="31211-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31211-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31211-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31211-106">一组设备配置策略的冲突摘要。</span><span class="sxs-lookup"><span data-stu-id="31211-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="methods"></a><span data-ttu-id="31211-107">方法</span><span class="sxs-lookup"><span data-stu-id="31211-107">Methods</span></span>
|<span data-ttu-id="31211-108">方法</span><span class="sxs-lookup"><span data-stu-id="31211-108">Method</span></span>|<span data-ttu-id="31211-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="31211-109">Return Type</span></span>|<span data-ttu-id="31211-110">说明</span><span class="sxs-lookup"><span data-stu-id="31211-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31211-111">列出 deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="31211-111">List deviceConfigurationConflictSummaries</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|<span data-ttu-id="31211-112">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="31211-112">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) collection</span></span>|<span data-ttu-id="31211-113">列出[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31211-113">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>|
|[<span data-ttu-id="31211-114">获取 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-114">Get deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[<span data-ttu-id="31211-115">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-115">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="31211-116">读取[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31211-116">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="31211-117">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-117">Create deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[<span data-ttu-id="31211-118">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-118">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="31211-119">创建新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31211-119">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|
|[<span data-ttu-id="31211-120">删除 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-120">Delete deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|<span data-ttu-id="31211-121">无</span><span class="sxs-lookup"><span data-stu-id="31211-121">None</span></span>|<span data-ttu-id="31211-122">删除[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="31211-122">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>|
|[<span data-ttu-id="31211-123">更新 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-123">Update deviceConfigurationConflictSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[<span data-ttu-id="31211-124">deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="31211-124">deviceConfigurationConflictSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|<span data-ttu-id="31211-125">更新[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="31211-125">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31211-126">属性</span><span class="sxs-lookup"><span data-stu-id="31211-126">Properties</span></span>
|<span data-ttu-id="31211-127">属性</span><span class="sxs-lookup"><span data-stu-id="31211-127">Property</span></span>|<span data-ttu-id="31211-128">类型</span><span class="sxs-lookup"><span data-stu-id="31211-128">Type</span></span>|<span data-ttu-id="31211-129">说明</span><span class="sxs-lookup"><span data-stu-id="31211-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31211-130">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="31211-130">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="31211-131">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31211-131">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="31211-132">与给定设置发生冲突的策略集</span><span class="sxs-lookup"><span data-stu-id="31211-132">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="31211-133">id</span><span class="sxs-lookup"><span data-stu-id="31211-133">id</span></span>|<span data-ttu-id="31211-134">String</span><span class="sxs-lookup"><span data-stu-id="31211-134">String</span></span>|<span data-ttu-id="31211-135">此组冲突策略的 id。</span><span class="sxs-lookup"><span data-stu-id="31211-135">The id for this set of conflicting policies.</span></span> <span data-ttu-id="31211-136">此 id 是 ConflictingDeviceConfigurations 中的所有策略的 id, 以字典顺序分隔, 由下划线分隔。</span><span class="sxs-lookup"><span data-stu-id="31211-136">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="31211-137">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="31211-137">contributingSettings</span></span>|<span data-ttu-id="31211-138">String collection</span><span class="sxs-lookup"><span data-stu-id="31211-138">String collection</span></span>|<span data-ttu-id="31211-139">与给定策略发生冲突的设置集</span><span class="sxs-lookup"><span data-stu-id="31211-139">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="31211-140">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="31211-140">deviceCheckinsImpacted</span></span>|<span data-ttu-id="31211-141">Int32</span><span class="sxs-lookup"><span data-stu-id="31211-141">Int32</span></span>|<span data-ttu-id="31211-142">受冲突策略和设置影响的签入次数</span><span class="sxs-lookup"><span data-stu-id="31211-142">The count of checkins impacted by the conflicting policies and settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="31211-143">关系</span><span class="sxs-lookup"><span data-stu-id="31211-143">Relationships</span></span>
<span data-ttu-id="31211-144">无</span><span class="sxs-lookup"><span data-stu-id="31211-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31211-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31211-145">JSON Representation</span></span>
<span data-ttu-id="31211-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31211-146">Here is a JSON representation of the resource.</span></span>
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






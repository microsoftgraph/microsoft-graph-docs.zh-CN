---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 78f8947a24a29b0ae4c53469306ada5141ee5ce5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847934"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a><span data-ttu-id="12de8-103">deviceComplianceScheduledActionForRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="12de8-103">deviceComplianceScheduledActionForRule resource type</span></span>

> <span data-ttu-id="12de8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12de8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12de8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12de8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12de8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12de8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12de8-107">计划的规则操作</span><span class="sxs-lookup"><span data-stu-id="12de8-107">Scheduled Action for Rule</span></span>
## <a name="methods"></a><span data-ttu-id="12de8-108">方法</span><span class="sxs-lookup"><span data-stu-id="12de8-108">Methods</span></span>
|<span data-ttu-id="12de8-109">方法</span><span class="sxs-lookup"><span data-stu-id="12de8-109">Method</span></span>|<span data-ttu-id="12de8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="12de8-110">Return Type</span></span>|<span data-ttu-id="12de8-111">说明</span><span class="sxs-lookup"><span data-stu-id="12de8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12de8-112">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="12de8-112">List deviceComplianceScheduledActionForRules</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|<span data-ttu-id="12de8-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12de8-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="12de8-114">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12de8-114">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>|
|[<span data-ttu-id="12de8-115">获取 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-115">Get deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[<span data-ttu-id="12de8-116">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-116">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="12de8-117">读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12de8-117">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="12de8-118">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-118">Create deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[<span data-ttu-id="12de8-119">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-119">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="12de8-120">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12de8-120">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="12de8-121">删除 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-121">Delete deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|<span data-ttu-id="12de8-122">无</span><span class="sxs-lookup"><span data-stu-id="12de8-122">None</span></span>|<span data-ttu-id="12de8-123">删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。</span><span class="sxs-lookup"><span data-stu-id="12de8-123">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>|
|[<span data-ttu-id="12de8-124">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-124">Update deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[<span data-ttu-id="12de8-125">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12de8-125">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="12de8-126">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12de8-126">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12de8-127">属性</span><span class="sxs-lookup"><span data-stu-id="12de8-127">Properties</span></span>
|<span data-ttu-id="12de8-128">属性</span><span class="sxs-lookup"><span data-stu-id="12de8-128">Property</span></span>|<span data-ttu-id="12de8-129">类型</span><span class="sxs-lookup"><span data-stu-id="12de8-129">Type</span></span>|<span data-ttu-id="12de8-130">说明</span><span class="sxs-lookup"><span data-stu-id="12de8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12de8-131">id</span><span class="sxs-lookup"><span data-stu-id="12de8-131">id</span></span>|<span data-ttu-id="12de8-132">String</span><span class="sxs-lookup"><span data-stu-id="12de8-132">String</span></span>|<span data-ttu-id="12de8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12de8-133">Key of the entity.</span></span>|
|<span data-ttu-id="12de8-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="12de8-134">ruleName</span></span>|<span data-ttu-id="12de8-135">String</span><span class="sxs-lookup"><span data-stu-id="12de8-135">String</span></span>|<span data-ttu-id="12de8-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="12de8-136">Name of the rule which this scheduled action applies to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12de8-137">关系</span><span class="sxs-lookup"><span data-stu-id="12de8-137">Relationships</span></span>
|<span data-ttu-id="12de8-138">关系</span><span class="sxs-lookup"><span data-stu-id="12de8-138">Relationship</span></span>|<span data-ttu-id="12de8-139">类型</span><span class="sxs-lookup"><span data-stu-id="12de8-139">Type</span></span>|<span data-ttu-id="12de8-140">说明</span><span class="sxs-lookup"><span data-stu-id="12de8-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12de8-141">scheduledActionConfigurations</span><span class="sxs-lookup"><span data-stu-id="12de8-141">scheduledActionConfigurations</span></span>|<span data-ttu-id="12de8-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12de8-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="12de8-143">此合规性策略的计划操作配置列表。</span><span class="sxs-lookup"><span data-stu-id="12de8-143">The list of scheduled action configurations for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12de8-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12de8-144">JSON Representation</span></span>
<span data-ttu-id="12de8-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12de8-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```






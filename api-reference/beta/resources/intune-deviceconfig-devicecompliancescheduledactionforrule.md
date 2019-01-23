---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2cb485b83ce11c3f3dcca51d11d9a0cfb977195
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425300"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a><span data-ttu-id="330ae-103">deviceComplianceScheduledActionForRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="330ae-103">deviceComplianceScheduledActionForRule resource type</span></span>

> <span data-ttu-id="330ae-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="330ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="330ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="330ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="330ae-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="330ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="330ae-107">计划的规则操作</span><span class="sxs-lookup"><span data-stu-id="330ae-107">Scheduled Action for Rule</span></span>

## <a name="methods"></a><span data-ttu-id="330ae-108">方法</span><span class="sxs-lookup"><span data-stu-id="330ae-108">Methods</span></span>
|<span data-ttu-id="330ae-109">方法</span><span class="sxs-lookup"><span data-stu-id="330ae-109">Method</span></span>|<span data-ttu-id="330ae-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="330ae-110">Return Type</span></span>|<span data-ttu-id="330ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="330ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="330ae-112">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="330ae-112">List deviceComplianceScheduledActionForRules</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|<span data-ttu-id="330ae-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="330ae-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="330ae-114">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="330ae-114">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>|
|[<span data-ttu-id="330ae-115">获取 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-115">Get deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[<span data-ttu-id="330ae-116">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-116">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="330ae-117">读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="330ae-117">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="330ae-118">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-118">Create deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[<span data-ttu-id="330ae-119">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-119">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="330ae-120">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="330ae-120">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="330ae-121">删除 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-121">Delete deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|<span data-ttu-id="330ae-122">无</span><span class="sxs-lookup"><span data-stu-id="330ae-122">None</span></span>|<span data-ttu-id="330ae-123">删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。</span><span class="sxs-lookup"><span data-stu-id="330ae-123">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>|
|[<span data-ttu-id="330ae-124">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-124">Update deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[<span data-ttu-id="330ae-125">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="330ae-125">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="330ae-126">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="330ae-126">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="330ae-127">属性</span><span class="sxs-lookup"><span data-stu-id="330ae-127">Properties</span></span>
|<span data-ttu-id="330ae-128">属性</span><span class="sxs-lookup"><span data-stu-id="330ae-128">Property</span></span>|<span data-ttu-id="330ae-129">类型</span><span class="sxs-lookup"><span data-stu-id="330ae-129">Type</span></span>|<span data-ttu-id="330ae-130">说明</span><span class="sxs-lookup"><span data-stu-id="330ae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330ae-131">id</span><span class="sxs-lookup"><span data-stu-id="330ae-131">id</span></span>|<span data-ttu-id="330ae-132">String</span><span class="sxs-lookup"><span data-stu-id="330ae-132">String</span></span>|<span data-ttu-id="330ae-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="330ae-133">Key of the entity.</span></span>|
|<span data-ttu-id="330ae-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="330ae-134">ruleName</span></span>|<span data-ttu-id="330ae-135">String</span><span class="sxs-lookup"><span data-stu-id="330ae-135">String</span></span>|<span data-ttu-id="330ae-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="330ae-136">Name of the rule which this scheduled action applies to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="330ae-137">关系</span><span class="sxs-lookup"><span data-stu-id="330ae-137">Relationships</span></span>
|<span data-ttu-id="330ae-138">关系</span><span class="sxs-lookup"><span data-stu-id="330ae-138">Relationship</span></span>|<span data-ttu-id="330ae-139">类型</span><span class="sxs-lookup"><span data-stu-id="330ae-139">Type</span></span>|<span data-ttu-id="330ae-140">说明</span><span class="sxs-lookup"><span data-stu-id="330ae-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330ae-141">scheduledActionConfigurations</span><span class="sxs-lookup"><span data-stu-id="330ae-141">scheduledActionConfigurations</span></span>|<span data-ttu-id="330ae-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="330ae-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="330ae-143">此合规性策略的计划操作配置列表。</span><span class="sxs-lookup"><span data-stu-id="330ae-143">The list of scheduled action configurations for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="330ae-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="330ae-144">JSON Representation</span></span>
<span data-ttu-id="330ae-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="330ae-145">Here is a JSON representation of the resource.</span></span>
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





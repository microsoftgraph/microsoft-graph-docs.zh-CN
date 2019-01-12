---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61e0fa49afaf3b048d1d10b1c06006cb0537f005
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965710"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a><span data-ttu-id="377e0-103">deviceComplianceScheduledActionForRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="377e0-103">deviceComplianceScheduledActionForRule resource type</span></span>

> <span data-ttu-id="377e0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="377e0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="377e0-105">计划的规则操作</span><span class="sxs-lookup"><span data-stu-id="377e0-105">Scheduled Action for Rule</span></span>
## <a name="methods"></a><span data-ttu-id="377e0-106">方法</span><span class="sxs-lookup"><span data-stu-id="377e0-106">Methods</span></span>
|<span data-ttu-id="377e0-107">方法</span><span class="sxs-lookup"><span data-stu-id="377e0-107">Method</span></span>|<span data-ttu-id="377e0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="377e0-108">Return Type</span></span>|<span data-ttu-id="377e0-109">说明</span><span class="sxs-lookup"><span data-stu-id="377e0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="377e0-110">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="377e0-110">List deviceComplianceScheduledActionForRules</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|<span data-ttu-id="377e0-111">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="377e0-111">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="377e0-112">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="377e0-112">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>|
|[<span data-ttu-id="377e0-113">获取 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-113">Get deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[<span data-ttu-id="377e0-114">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-114">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="377e0-115">读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="377e0-115">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="377e0-116">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-116">Create deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[<span data-ttu-id="377e0-117">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-117">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="377e0-118">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="377e0-118">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="377e0-119">删除 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-119">Delete deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|<span data-ttu-id="377e0-120">无</span><span class="sxs-lookup"><span data-stu-id="377e0-120">None</span></span>|<span data-ttu-id="377e0-121">删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。</span><span class="sxs-lookup"><span data-stu-id="377e0-121">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>|
|[<span data-ttu-id="377e0-122">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-122">Update deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[<span data-ttu-id="377e0-123">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="377e0-123">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="377e0-124">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="377e0-124">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="377e0-125">属性</span><span class="sxs-lookup"><span data-stu-id="377e0-125">Properties</span></span>
|<span data-ttu-id="377e0-126">属性</span><span class="sxs-lookup"><span data-stu-id="377e0-126">Property</span></span>|<span data-ttu-id="377e0-127">类型</span><span class="sxs-lookup"><span data-stu-id="377e0-127">Type</span></span>|<span data-ttu-id="377e0-128">说明</span><span class="sxs-lookup"><span data-stu-id="377e0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="377e0-129">id</span><span class="sxs-lookup"><span data-stu-id="377e0-129">id</span></span>|<span data-ttu-id="377e0-130">String</span><span class="sxs-lookup"><span data-stu-id="377e0-130">String</span></span>|<span data-ttu-id="377e0-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="377e0-131">Key of the entity.</span></span>|
|<span data-ttu-id="377e0-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="377e0-132">ruleName</span></span>|<span data-ttu-id="377e0-133">String</span><span class="sxs-lookup"><span data-stu-id="377e0-133">String</span></span>|<span data-ttu-id="377e0-134">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="377e0-134">Name of the rule which this scheduled action applies to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="377e0-135">关系</span><span class="sxs-lookup"><span data-stu-id="377e0-135">Relationships</span></span>
|<span data-ttu-id="377e0-136">关系</span><span class="sxs-lookup"><span data-stu-id="377e0-136">Relationship</span></span>|<span data-ttu-id="377e0-137">类型</span><span class="sxs-lookup"><span data-stu-id="377e0-137">Type</span></span>|<span data-ttu-id="377e0-138">说明</span><span class="sxs-lookup"><span data-stu-id="377e0-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="377e0-139">scheduledActionConfigurations</span><span class="sxs-lookup"><span data-stu-id="377e0-139">scheduledActionConfigurations</span></span>|<span data-ttu-id="377e0-140">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="377e0-140">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="377e0-141">此合规性策略的计划操作配置列表。</span><span class="sxs-lookup"><span data-stu-id="377e0-141">The list of scheduled action configurations for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="377e0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="377e0-142">JSON Representation</span></span>
<span data-ttu-id="377e0-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="377e0-143">Here is a JSON representation of the resource.</span></span>
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




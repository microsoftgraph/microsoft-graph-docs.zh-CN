---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
ms.openlocfilehash: afb2544312a90c2cea0855ad6f0b91f8bbdd74fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041501"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a><span data-ttu-id="80213-103">deviceComplianceScheduledActionForRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="80213-103">deviceComplianceScheduledActionForRule resource type</span></span>

> <span data-ttu-id="80213-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80213-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80213-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80213-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80213-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80213-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80213-107">计划的规则操作</span><span class="sxs-lookup"><span data-stu-id="80213-107">Scheduled Action for Rule</span></span>
## <a name="methods"></a><span data-ttu-id="80213-108">方法</span><span class="sxs-lookup"><span data-stu-id="80213-108">Methods</span></span>
|<span data-ttu-id="80213-109">方法</span><span class="sxs-lookup"><span data-stu-id="80213-109">Method</span></span>|<span data-ttu-id="80213-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="80213-110">Return Type</span></span>|<span data-ttu-id="80213-111">说明</span><span class="sxs-lookup"><span data-stu-id="80213-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80213-112">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="80213-112">List deviceComplianceScheduledActionForRules</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|<span data-ttu-id="80213-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80213-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="80213-114">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80213-114">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>|
|[<span data-ttu-id="80213-115">获取 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-115">Get deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[<span data-ttu-id="80213-116">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-116">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="80213-117">读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80213-117">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="80213-118">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-118">Create deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[<span data-ttu-id="80213-119">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-119">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="80213-120">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80213-120">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="80213-121">删除 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-121">Delete deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|<span data-ttu-id="80213-122">无</span><span class="sxs-lookup"><span data-stu-id="80213-122">None</span></span>|<span data-ttu-id="80213-123">删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。</span><span class="sxs-lookup"><span data-stu-id="80213-123">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>|
|[<span data-ttu-id="80213-124">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-124">Update deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[<span data-ttu-id="80213-125">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="80213-125">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="80213-126">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80213-126">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80213-127">属性</span><span class="sxs-lookup"><span data-stu-id="80213-127">Properties</span></span>
|<span data-ttu-id="80213-128">属性</span><span class="sxs-lookup"><span data-stu-id="80213-128">Property</span></span>|<span data-ttu-id="80213-129">类型</span><span class="sxs-lookup"><span data-stu-id="80213-129">Type</span></span>|<span data-ttu-id="80213-130">说明</span><span class="sxs-lookup"><span data-stu-id="80213-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80213-131">id</span><span class="sxs-lookup"><span data-stu-id="80213-131">id</span></span>|<span data-ttu-id="80213-132">String</span><span class="sxs-lookup"><span data-stu-id="80213-132">String</span></span>|<span data-ttu-id="80213-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80213-133">Key of the entity.</span></span>|
|<span data-ttu-id="80213-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="80213-134">ruleName</span></span>|<span data-ttu-id="80213-135">String</span><span class="sxs-lookup"><span data-stu-id="80213-135">String</span></span>|<span data-ttu-id="80213-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="80213-136">Name of the rule which this scheduled action applies to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80213-137">关系</span><span class="sxs-lookup"><span data-stu-id="80213-137">Relationships</span></span>
|<span data-ttu-id="80213-138">关系</span><span class="sxs-lookup"><span data-stu-id="80213-138">Relationship</span></span>|<span data-ttu-id="80213-139">类型</span><span class="sxs-lookup"><span data-stu-id="80213-139">Type</span></span>|<span data-ttu-id="80213-140">说明</span><span class="sxs-lookup"><span data-stu-id="80213-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80213-141">scheduledActionConfigurations</span><span class="sxs-lookup"><span data-stu-id="80213-141">scheduledActionConfigurations</span></span>|<span data-ttu-id="80213-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80213-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="80213-143">此合规性策略的计划操作配置列表。</span><span class="sxs-lookup"><span data-stu-id="80213-143">The list of scheduled action configurations for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80213-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80213-144">JSON Representation</span></span>
<span data-ttu-id="80213-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80213-145">Here is a JSON representation of the resource.</span></span>
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






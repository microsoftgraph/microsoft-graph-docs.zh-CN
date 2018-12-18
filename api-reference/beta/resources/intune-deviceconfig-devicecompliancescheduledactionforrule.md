---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
author: tfitzmac
ms.openlocfilehash: 912a0722b85857aa64daa5339cc7730a4c0413ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344770"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a><span data-ttu-id="b327b-103">deviceComplianceScheduledActionForRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="b327b-103">deviceComplianceScheduledActionForRule resource type</span></span>

> <span data-ttu-id="b327b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b327b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b327b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b327b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b327b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b327b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b327b-107">计划的规则操作</span><span class="sxs-lookup"><span data-stu-id="b327b-107">Scheduled Action for Rule</span></span>
## <a name="methods"></a><span data-ttu-id="b327b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b327b-108">Methods</span></span>
|<span data-ttu-id="b327b-109">方法</span><span class="sxs-lookup"><span data-stu-id="b327b-109">Method</span></span>|<span data-ttu-id="b327b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b327b-110">Return Type</span></span>|<span data-ttu-id="b327b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b327b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b327b-112">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="b327b-112">List deviceComplianceScheduledActionForRules</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|<span data-ttu-id="b327b-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b327b-113">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="b327b-114">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b327b-114">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>|
|[<span data-ttu-id="b327b-115">获取 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-115">Get deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[<span data-ttu-id="b327b-116">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-116">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="b327b-117">读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b327b-117">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="b327b-118">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-118">Create deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[<span data-ttu-id="b327b-119">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-119">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="b327b-120">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b327b-120">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|
|[<span data-ttu-id="b327b-121">删除 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-121">Delete deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|<span data-ttu-id="b327b-122">无</span><span class="sxs-lookup"><span data-stu-id="b327b-122">None</span></span>|<span data-ttu-id="b327b-123">删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。</span><span class="sxs-lookup"><span data-stu-id="b327b-123">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>|
|[<span data-ttu-id="b327b-124">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-124">Update deviceComplianceScheduledActionForRule</span></span>](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[<span data-ttu-id="b327b-125">deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="b327b-125">deviceComplianceScheduledActionForRule</span></span>](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|<span data-ttu-id="b327b-126">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b327b-126">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b327b-127">属性</span><span class="sxs-lookup"><span data-stu-id="b327b-127">Properties</span></span>
|<span data-ttu-id="b327b-128">属性</span><span class="sxs-lookup"><span data-stu-id="b327b-128">Property</span></span>|<span data-ttu-id="b327b-129">类型</span><span class="sxs-lookup"><span data-stu-id="b327b-129">Type</span></span>|<span data-ttu-id="b327b-130">说明</span><span class="sxs-lookup"><span data-stu-id="b327b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b327b-131">id</span><span class="sxs-lookup"><span data-stu-id="b327b-131">id</span></span>|<span data-ttu-id="b327b-132">String</span><span class="sxs-lookup"><span data-stu-id="b327b-132">String</span></span>|<span data-ttu-id="b327b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b327b-133">Key of the entity.</span></span>|
|<span data-ttu-id="b327b-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="b327b-134">ruleName</span></span>|<span data-ttu-id="b327b-135">String</span><span class="sxs-lookup"><span data-stu-id="b327b-135">String</span></span>|<span data-ttu-id="b327b-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="b327b-136">Name of the rule which this scheduled action applies to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b327b-137">关系</span><span class="sxs-lookup"><span data-stu-id="b327b-137">Relationships</span></span>
|<span data-ttu-id="b327b-138">关系</span><span class="sxs-lookup"><span data-stu-id="b327b-138">Relationship</span></span>|<span data-ttu-id="b327b-139">类型</span><span class="sxs-lookup"><span data-stu-id="b327b-139">Type</span></span>|<span data-ttu-id="b327b-140">说明</span><span class="sxs-lookup"><span data-stu-id="b327b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b327b-141">scheduledActionConfigurations</span><span class="sxs-lookup"><span data-stu-id="b327b-141">scheduledActionConfigurations</span></span>|<span data-ttu-id="b327b-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b327b-142">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="b327b-143">此合规性策略的计划操作配置列表。</span><span class="sxs-lookup"><span data-stu-id="b327b-143">The list of scheduled action configurations for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b327b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b327b-144">JSON Representation</span></span>
<span data-ttu-id="b327b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b327b-145">Here is a JSON representation of the resource.</span></span>
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






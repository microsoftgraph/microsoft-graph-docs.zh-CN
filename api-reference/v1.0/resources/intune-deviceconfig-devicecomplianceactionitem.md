---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbb67151b38f6c65bf8abae1b16a96b8cb25584f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845806"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="b42a9-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b42a9-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="b42a9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b42a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b42a9-105">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="b42a9-105">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="b42a9-106">方法</span><span class="sxs-lookup"><span data-stu-id="b42a9-106">Methods</span></span>
|<span data-ttu-id="b42a9-107">方法</span><span class="sxs-lookup"><span data-stu-id="b42a9-107">Method</span></span>|<span data-ttu-id="b42a9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b42a9-108">Return Type</span></span>|<span data-ttu-id="b42a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="b42a9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b42a9-110">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="b42a9-110">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="b42a9-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b42a9-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="b42a9-112">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b42a9-112">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="b42a9-113">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-113">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="b42a9-114">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-114">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b42a9-115">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b42a9-115">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="b42a9-116">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-116">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="b42a9-117">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-117">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b42a9-118">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b42a9-118">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="b42a9-119">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-119">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="b42a9-120">无</span><span class="sxs-lookup"><span data-stu-id="b42a9-120">None</span></span>|<span data-ttu-id="b42a9-121">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b42a9-121">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="b42a9-122">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-122">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="b42a9-123">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b42a9-123">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b42a9-124">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b42a9-124">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b42a9-125">属性</span><span class="sxs-lookup"><span data-stu-id="b42a9-125">Properties</span></span>
|<span data-ttu-id="b42a9-126">属性</span><span class="sxs-lookup"><span data-stu-id="b42a9-126">Property</span></span>|<span data-ttu-id="b42a9-127">类型</span><span class="sxs-lookup"><span data-stu-id="b42a9-127">Type</span></span>|<span data-ttu-id="b42a9-128">说明</span><span class="sxs-lookup"><span data-stu-id="b42a9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b42a9-129">id</span><span class="sxs-lookup"><span data-stu-id="b42a9-129">id</span></span>|<span data-ttu-id="b42a9-130">String</span><span class="sxs-lookup"><span data-stu-id="b42a9-130">String</span></span>|<span data-ttu-id="b42a9-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b42a9-131">Key of the entity.</span></span>|
|<span data-ttu-id="b42a9-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="b42a9-132">gracePeriodHours</span></span>|<span data-ttu-id="b42a9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b42a9-133">Int32</span></span>|<span data-ttu-id="b42a9-134">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="b42a9-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="b42a9-135">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="b42a9-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="b42a9-136">actionType</span><span class="sxs-lookup"><span data-stu-id="b42a9-136">actionType</span></span>|[<span data-ttu-id="b42a9-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="b42a9-137">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="b42a9-138">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="b42a9-138">What action to take.</span></span> <span data-ttu-id="b42a9-139">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`。</span><span class="sxs-lookup"><span data-stu-id="b42a9-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="b42a9-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="b42a9-140">notificationTemplateId</span></span>|<span data-ttu-id="b42a9-141">String</span><span class="sxs-lookup"><span data-stu-id="b42a9-141">String</span></span>|<span data-ttu-id="b42a9-142">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="b42a9-142">What notification Message template to use</span></span>|
|<span data-ttu-id="b42a9-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="b42a9-143">notificationMessageCCList</span></span>|<span data-ttu-id="b42a9-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="b42a9-144">String collection</span></span>|<span data-ttu-id="b42a9-145">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b42a9-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b42a9-146">关系</span><span class="sxs-lookup"><span data-stu-id="b42a9-146">Relationships</span></span>
<span data-ttu-id="b42a9-147">无</span><span class="sxs-lookup"><span data-stu-id="b42a9-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b42a9-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b42a9-148">JSON Representation</span></span>
<span data-ttu-id="b42a9-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b42a9-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```




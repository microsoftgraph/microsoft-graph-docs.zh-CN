---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6a96ca90ee9967968799e2bc1bea281346eaf1c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414961"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="4d324-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d324-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="4d324-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4d324-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d324-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d324-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d324-107">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="4d324-107">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="4d324-108">方法</span><span class="sxs-lookup"><span data-stu-id="4d324-108">Methods</span></span>
|<span data-ttu-id="4d324-109">方法</span><span class="sxs-lookup"><span data-stu-id="4d324-109">Method</span></span>|<span data-ttu-id="4d324-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d324-110">Return Type</span></span>|<span data-ttu-id="4d324-111">说明</span><span class="sxs-lookup"><span data-stu-id="4d324-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d324-112">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="4d324-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="4d324-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d324-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="4d324-114">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d324-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="4d324-115">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="4d324-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4d324-117">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d324-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="4d324-118">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="4d324-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4d324-120">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d324-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="4d324-121">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="4d324-122">无</span><span class="sxs-lookup"><span data-stu-id="4d324-122">None</span></span>|<span data-ttu-id="4d324-123">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4d324-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="4d324-124">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="4d324-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="4d324-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="4d324-126">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d324-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d324-127">属性</span><span class="sxs-lookup"><span data-stu-id="4d324-127">Properties</span></span>
|<span data-ttu-id="4d324-128">属性</span><span class="sxs-lookup"><span data-stu-id="4d324-128">Property</span></span>|<span data-ttu-id="4d324-129">类型</span><span class="sxs-lookup"><span data-stu-id="4d324-129">Type</span></span>|<span data-ttu-id="4d324-130">说明</span><span class="sxs-lookup"><span data-stu-id="4d324-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d324-131">id</span><span class="sxs-lookup"><span data-stu-id="4d324-131">id</span></span>|<span data-ttu-id="4d324-132">String</span><span class="sxs-lookup"><span data-stu-id="4d324-132">String</span></span>|<span data-ttu-id="4d324-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d324-133">Key of the entity.</span></span>|
|<span data-ttu-id="4d324-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="4d324-134">gracePeriodHours</span></span>|<span data-ttu-id="4d324-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4d324-135">Int32</span></span>|<span data-ttu-id="4d324-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="4d324-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="4d324-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="4d324-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="4d324-138">actionType</span><span class="sxs-lookup"><span data-stu-id="4d324-138">actionType</span></span>|[<span data-ttu-id="4d324-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="4d324-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="4d324-140">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="4d324-140">What action to take.</span></span> <span data-ttu-id="4d324-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="4d324-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="4d324-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="4d324-142">notificationTemplateId</span></span>|<span data-ttu-id="4d324-143">String</span><span class="sxs-lookup"><span data-stu-id="4d324-143">String</span></span>|<span data-ttu-id="4d324-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="4d324-144">What notification Message template to use</span></span>|
|<span data-ttu-id="4d324-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="4d324-145">notificationMessageCCList</span></span>|<span data-ttu-id="4d324-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="4d324-146">String collection</span></span>|<span data-ttu-id="4d324-147">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="4d324-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d324-148">关系</span><span class="sxs-lookup"><span data-stu-id="4d324-148">Relationships</span></span>
<span data-ttu-id="4d324-149">无</span><span class="sxs-lookup"><span data-stu-id="4d324-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d324-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d324-150">JSON Representation</span></span>
<span data-ttu-id="4d324-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d324-151">Here is a JSON representation of the resource.</span></span>
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





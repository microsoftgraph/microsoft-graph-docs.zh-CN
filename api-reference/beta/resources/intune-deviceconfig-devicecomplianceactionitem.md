---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d1aa888b926cd0e9d4435e23b0b281618978d2e2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216183"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="9a5af-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a5af-103">deviceComplianceActionItem resource type</span></span>

<span data-ttu-id="9a5af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a5af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a5af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a5af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a5af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a5af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a5af-107">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="9a5af-107">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="9a5af-108">方法</span><span class="sxs-lookup"><span data-stu-id="9a5af-108">Methods</span></span>
|<span data-ttu-id="9a5af-109">方法</span><span class="sxs-lookup"><span data-stu-id="9a5af-109">Method</span></span>|<span data-ttu-id="9a5af-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a5af-110">Return Type</span></span>|<span data-ttu-id="9a5af-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a5af-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9a5af-112">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="9a5af-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="9a5af-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a5af-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="9a5af-114">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a5af-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="9a5af-115">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="9a5af-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9a5af-117">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a5af-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9a5af-118">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="9a5af-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9a5af-120">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a5af-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9a5af-121">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="9a5af-122">无</span><span class="sxs-lookup"><span data-stu-id="9a5af-122">None</span></span>|<span data-ttu-id="9a5af-123">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9a5af-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="9a5af-124">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="9a5af-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9a5af-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9a5af-126">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a5af-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a5af-127">属性</span><span class="sxs-lookup"><span data-stu-id="9a5af-127">Properties</span></span>
|<span data-ttu-id="9a5af-128">属性</span><span class="sxs-lookup"><span data-stu-id="9a5af-128">Property</span></span>|<span data-ttu-id="9a5af-129">类型</span><span class="sxs-lookup"><span data-stu-id="9a5af-129">Type</span></span>|<span data-ttu-id="9a5af-130">说明</span><span class="sxs-lookup"><span data-stu-id="9a5af-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a5af-131">id</span><span class="sxs-lookup"><span data-stu-id="9a5af-131">id</span></span>|<span data-ttu-id="9a5af-132">String</span><span class="sxs-lookup"><span data-stu-id="9a5af-132">String</span></span>|<span data-ttu-id="9a5af-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9a5af-133">Key of the entity.</span></span>|
|<span data-ttu-id="9a5af-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9a5af-134">gracePeriodHours</span></span>|<span data-ttu-id="9a5af-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9a5af-135">Int32</span></span>|<span data-ttu-id="9a5af-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="9a5af-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9a5af-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="9a5af-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9a5af-138">actionType</span><span class="sxs-lookup"><span data-stu-id="9a5af-138">actionType</span></span>|[<span data-ttu-id="9a5af-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9a5af-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9a5af-140">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="9a5af-140">What action to take.</span></span> <span data-ttu-id="9a5af-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="9a5af-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="9a5af-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9a5af-142">notificationTemplateId</span></span>|<span data-ttu-id="9a5af-143">String</span><span class="sxs-lookup"><span data-stu-id="9a5af-143">String</span></span>|<span data-ttu-id="9a5af-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="9a5af-144">What notification Message template to use</span></span>|
|<span data-ttu-id="9a5af-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9a5af-145">notificationMessageCCList</span></span>|<span data-ttu-id="9a5af-146">String collection</span><span class="sxs-lookup"><span data-stu-id="9a5af-146">String collection</span></span>|<span data-ttu-id="9a5af-147">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9a5af-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a5af-148">关系</span><span class="sxs-lookup"><span data-stu-id="9a5af-148">Relationships</span></span>
<span data-ttu-id="9a5af-149">无</span><span class="sxs-lookup"><span data-stu-id="9a5af-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a5af-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a5af-150">JSON Representation</span></span>
<span data-ttu-id="9a5af-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a5af-151">Here is a JSON representation of the resource.</span></span>
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





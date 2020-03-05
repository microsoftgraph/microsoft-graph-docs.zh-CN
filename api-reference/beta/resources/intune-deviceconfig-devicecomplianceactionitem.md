---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3962864aa220cd3231d69b0b069cc37342f192ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526727"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="b9608-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9608-103">deviceComplianceActionItem resource type</span></span>

<span data-ttu-id="b9608-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b9608-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9608-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9608-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9608-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9608-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9608-107">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="b9608-107">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="b9608-108">方法</span><span class="sxs-lookup"><span data-stu-id="b9608-108">Methods</span></span>
|<span data-ttu-id="b9608-109">方法</span><span class="sxs-lookup"><span data-stu-id="b9608-109">Method</span></span>|<span data-ttu-id="b9608-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9608-110">Return Type</span></span>|<span data-ttu-id="b9608-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9608-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9608-112">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="b9608-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="b9608-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9608-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="b9608-114">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9608-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="b9608-115">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="b9608-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b9608-117">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9608-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="b9608-118">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="b9608-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b9608-120">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9608-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="b9608-121">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="b9608-122">无</span><span class="sxs-lookup"><span data-stu-id="b9608-122">None</span></span>|<span data-ttu-id="b9608-123">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b9608-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="b9608-124">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="b9608-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b9608-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="b9608-126">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9608-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9608-127">属性</span><span class="sxs-lookup"><span data-stu-id="b9608-127">Properties</span></span>
|<span data-ttu-id="b9608-128">属性</span><span class="sxs-lookup"><span data-stu-id="b9608-128">Property</span></span>|<span data-ttu-id="b9608-129">类型</span><span class="sxs-lookup"><span data-stu-id="b9608-129">Type</span></span>|<span data-ttu-id="b9608-130">说明</span><span class="sxs-lookup"><span data-stu-id="b9608-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9608-131">id</span><span class="sxs-lookup"><span data-stu-id="b9608-131">id</span></span>|<span data-ttu-id="b9608-132">String</span><span class="sxs-lookup"><span data-stu-id="b9608-132">String</span></span>|<span data-ttu-id="b9608-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9608-133">Key of the entity.</span></span>|
|<span data-ttu-id="b9608-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="b9608-134">gracePeriodHours</span></span>|<span data-ttu-id="b9608-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b9608-135">Int32</span></span>|<span data-ttu-id="b9608-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="b9608-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="b9608-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="b9608-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="b9608-138">actionType</span><span class="sxs-lookup"><span data-stu-id="b9608-138">actionType</span></span>|[<span data-ttu-id="b9608-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="b9608-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="b9608-140">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="b9608-140">What action to take.</span></span> <span data-ttu-id="b9608-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="b9608-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="b9608-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="b9608-142">notificationTemplateId</span></span>|<span data-ttu-id="b9608-143">String</span><span class="sxs-lookup"><span data-stu-id="b9608-143">String</span></span>|<span data-ttu-id="b9608-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="b9608-144">What notification Message template to use</span></span>|
|<span data-ttu-id="b9608-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="b9608-145">notificationMessageCCList</span></span>|<span data-ttu-id="b9608-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b9608-146">String collection</span></span>|<span data-ttu-id="b9608-147">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b9608-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9608-148">关系</span><span class="sxs-lookup"><span data-stu-id="b9608-148">Relationships</span></span>
<span data-ttu-id="b9608-149">无</span><span class="sxs-lookup"><span data-stu-id="b9608-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9608-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9608-150">JSON Representation</span></span>
<span data-ttu-id="b9608-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9608-151">Here is a JSON representation of the resource.</span></span>
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




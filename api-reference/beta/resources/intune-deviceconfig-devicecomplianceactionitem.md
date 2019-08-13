---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4a8e58d083f0985164d34607a9b7970025dee1e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333224"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="96a4e-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="96a4e-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="96a4e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96a4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96a4e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96a4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a4e-106">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="96a4e-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="96a4e-107">方法</span><span class="sxs-lookup"><span data-stu-id="96a4e-107">Methods</span></span>
|<span data-ttu-id="96a4e-108">方法</span><span class="sxs-lookup"><span data-stu-id="96a4e-108">Method</span></span>|<span data-ttu-id="96a4e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="96a4e-109">Return Type</span></span>|<span data-ttu-id="96a4e-110">说明</span><span class="sxs-lookup"><span data-stu-id="96a4e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96a4e-111">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="96a4e-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="96a4e-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96a4e-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="96a4e-113">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96a4e-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="96a4e-114">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="96a4e-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="96a4e-116">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96a4e-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="96a4e-117">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="96a4e-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="96a4e-119">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96a4e-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="96a4e-120">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="96a4e-121">无</span><span class="sxs-lookup"><span data-stu-id="96a4e-121">None</span></span>|<span data-ttu-id="96a4e-122">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="96a4e-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="96a4e-123">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="96a4e-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="96a4e-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="96a4e-125">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="96a4e-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96a4e-126">属性</span><span class="sxs-lookup"><span data-stu-id="96a4e-126">Properties</span></span>
|<span data-ttu-id="96a4e-127">属性</span><span class="sxs-lookup"><span data-stu-id="96a4e-127">Property</span></span>|<span data-ttu-id="96a4e-128">类型</span><span class="sxs-lookup"><span data-stu-id="96a4e-128">Type</span></span>|<span data-ttu-id="96a4e-129">说明</span><span class="sxs-lookup"><span data-stu-id="96a4e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a4e-130">id</span><span class="sxs-lookup"><span data-stu-id="96a4e-130">id</span></span>|<span data-ttu-id="96a4e-131">String</span><span class="sxs-lookup"><span data-stu-id="96a4e-131">String</span></span>|<span data-ttu-id="96a4e-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="96a4e-132">Key of the entity.</span></span>|
|<span data-ttu-id="96a4e-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="96a4e-133">gracePeriodHours</span></span>|<span data-ttu-id="96a4e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="96a4e-134">Int32</span></span>|<span data-ttu-id="96a4e-135">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="96a4e-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="96a4e-136">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="96a4e-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="96a4e-137">actionType</span><span class="sxs-lookup"><span data-stu-id="96a4e-137">actionType</span></span>|[<span data-ttu-id="96a4e-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="96a4e-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="96a4e-139">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="96a4e-139">What action to take.</span></span> <span data-ttu-id="96a4e-140">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="96a4e-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="96a4e-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="96a4e-141">notificationTemplateId</span></span>|<span data-ttu-id="96a4e-142">String</span><span class="sxs-lookup"><span data-stu-id="96a4e-142">String</span></span>|<span data-ttu-id="96a4e-143">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="96a4e-143">What notification Message template to use</span></span>|
|<span data-ttu-id="96a4e-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="96a4e-144">notificationMessageCCList</span></span>|<span data-ttu-id="96a4e-145">String collection</span><span class="sxs-lookup"><span data-stu-id="96a4e-145">String collection</span></span>|<span data-ttu-id="96a4e-146">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="96a4e-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a4e-147">关系</span><span class="sxs-lookup"><span data-stu-id="96a4e-147">Relationships</span></span>
<span data-ttu-id="96a4e-148">无</span><span class="sxs-lookup"><span data-stu-id="96a4e-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a4e-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96a4e-149">JSON Representation</span></span>
<span data-ttu-id="96a4e-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96a4e-150">Here is a JSON representation of the resource.</span></span>
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




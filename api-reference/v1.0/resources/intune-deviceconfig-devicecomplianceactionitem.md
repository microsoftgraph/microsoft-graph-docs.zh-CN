---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 386012b71373bf8acae03ea7026ecbddd5327daa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758867"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="06f86-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="06f86-103">deviceComplianceActionItem resource type</span></span>

<span data-ttu-id="06f86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06f86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06f86-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06f86-106">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="06f86-106">Scheduled Action Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="06f86-107">方法</span><span class="sxs-lookup"><span data-stu-id="06f86-107">Methods</span></span>
|<span data-ttu-id="06f86-108">方法</span><span class="sxs-lookup"><span data-stu-id="06f86-108">Method</span></span>|<span data-ttu-id="06f86-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="06f86-109">Return Type</span></span>|<span data-ttu-id="06f86-110">说明</span><span class="sxs-lookup"><span data-stu-id="06f86-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06f86-111">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="06f86-111">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="06f86-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06f86-112">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="06f86-113">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06f86-113">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="06f86-114">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-114">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="06f86-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-115">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="06f86-116">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06f86-116">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="06f86-117">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-117">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="06f86-118">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-118">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="06f86-119">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06f86-119">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="06f86-120">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-120">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="06f86-121">无</span><span class="sxs-lookup"><span data-stu-id="06f86-121">None</span></span>|<span data-ttu-id="06f86-122">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="06f86-122">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="06f86-123">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-123">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="06f86-124">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="06f86-124">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="06f86-125">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06f86-125">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06f86-126">属性</span><span class="sxs-lookup"><span data-stu-id="06f86-126">Properties</span></span>
|<span data-ttu-id="06f86-127">属性</span><span class="sxs-lookup"><span data-stu-id="06f86-127">Property</span></span>|<span data-ttu-id="06f86-128">类型</span><span class="sxs-lookup"><span data-stu-id="06f86-128">Type</span></span>|<span data-ttu-id="06f86-129">说明</span><span class="sxs-lookup"><span data-stu-id="06f86-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f86-130">id</span><span class="sxs-lookup"><span data-stu-id="06f86-130">id</span></span>|<span data-ttu-id="06f86-131">String</span><span class="sxs-lookup"><span data-stu-id="06f86-131">String</span></span>|<span data-ttu-id="06f86-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06f86-132">Key of the entity.</span></span>|
|<span data-ttu-id="06f86-133">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="06f86-133">gracePeriodHours</span></span>|<span data-ttu-id="06f86-134">Int32</span><span class="sxs-lookup"><span data-stu-id="06f86-134">Int32</span></span>|<span data-ttu-id="06f86-135">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="06f86-135">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="06f86-136">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="06f86-136">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="06f86-137">actionType</span><span class="sxs-lookup"><span data-stu-id="06f86-137">actionType</span></span>|[<span data-ttu-id="06f86-138">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="06f86-138">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="06f86-139">要采取哪些操作。</span><span class="sxs-lookup"><span data-stu-id="06f86-139">What action to take.</span></span> <span data-ttu-id="06f86-140">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles` 或 `pushNotification`。</span><span class="sxs-lookup"><span data-stu-id="06f86-140">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="06f86-141">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="06f86-141">notificationTemplateId</span></span>|<span data-ttu-id="06f86-142">String</span><span class="sxs-lookup"><span data-stu-id="06f86-142">String</span></span>|<span data-ttu-id="06f86-143">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="06f86-143">What notification Message template to use</span></span>|
|<span data-ttu-id="06f86-144">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="06f86-144">notificationMessageCCList</span></span>|<span data-ttu-id="06f86-145">String collection</span><span class="sxs-lookup"><span data-stu-id="06f86-145">String collection</span></span>|<span data-ttu-id="06f86-146">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="06f86-146">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06f86-147">关系</span><span class="sxs-lookup"><span data-stu-id="06f86-147">Relationships</span></span>
<span data-ttu-id="06f86-148">无</span><span class="sxs-lookup"><span data-stu-id="06f86-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06f86-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06f86-149">JSON Representation</span></span>
<span data-ttu-id="06f86-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06f86-150">Here is a JSON representation of the resource.</span></span>
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





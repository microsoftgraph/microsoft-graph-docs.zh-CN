---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: tfitzmac
ms.openlocfilehash: 0b9d9ba9a4b480da0891545f1f88eaa085a71e13
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312059"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="9f89c-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f89c-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="9f89c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f89c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f89c-105">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="9f89c-105">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="9f89c-106">方法</span><span class="sxs-lookup"><span data-stu-id="9f89c-106">Methods</span></span>
|<span data-ttu-id="9f89c-107">方法</span><span class="sxs-lookup"><span data-stu-id="9f89c-107">Method</span></span>|<span data-ttu-id="9f89c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f89c-108">Return Type</span></span>|<span data-ttu-id="9f89c-109">说明</span><span class="sxs-lookup"><span data-stu-id="9f89c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f89c-110">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="9f89c-110">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="9f89c-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f89c-111">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="9f89c-112">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f89c-112">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="9f89c-113">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-113">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="9f89c-114">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-114">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9f89c-115">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f89c-115">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9f89c-116">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-116">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="9f89c-117">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-117">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9f89c-118">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f89c-118">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9f89c-119">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-119">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="9f89c-120">无</span><span class="sxs-lookup"><span data-stu-id="9f89c-120">None</span></span>|<span data-ttu-id="9f89c-121">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9f89c-121">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="9f89c-122">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-122">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="9f89c-123">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9f89c-123">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9f89c-124">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f89c-124">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f89c-125">属性</span><span class="sxs-lookup"><span data-stu-id="9f89c-125">Properties</span></span>
|<span data-ttu-id="9f89c-126">属性</span><span class="sxs-lookup"><span data-stu-id="9f89c-126">Property</span></span>|<span data-ttu-id="9f89c-127">类型</span><span class="sxs-lookup"><span data-stu-id="9f89c-127">Type</span></span>|<span data-ttu-id="9f89c-128">说明</span><span class="sxs-lookup"><span data-stu-id="9f89c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f89c-129">id</span><span class="sxs-lookup"><span data-stu-id="9f89c-129">id</span></span>|<span data-ttu-id="9f89c-130">String</span><span class="sxs-lookup"><span data-stu-id="9f89c-130">String</span></span>|<span data-ttu-id="9f89c-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f89c-131">Key of the entity.</span></span>|
|<span data-ttu-id="9f89c-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9f89c-132">gracePeriodHours</span></span>|<span data-ttu-id="9f89c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9f89c-133">Int32</span></span>|<span data-ttu-id="9f89c-134">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="9f89c-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9f89c-135">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="9f89c-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9f89c-136">actionType</span><span class="sxs-lookup"><span data-stu-id="9f89c-136">actionType</span></span>|[<span data-ttu-id="9f89c-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9f89c-137">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9f89c-138">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="9f89c-138">What action to take.</span></span> <span data-ttu-id="9f89c-139">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`。</span><span class="sxs-lookup"><span data-stu-id="9f89c-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="9f89c-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9f89c-140">notificationTemplateId</span></span>|<span data-ttu-id="9f89c-141">String</span><span class="sxs-lookup"><span data-stu-id="9f89c-141">String</span></span>|<span data-ttu-id="9f89c-142">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="9f89c-142">What notification Message template to use</span></span>|
|<span data-ttu-id="9f89c-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9f89c-143">notificationMessageCCList</span></span>|<span data-ttu-id="9f89c-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f89c-144">String collection</span></span>|<span data-ttu-id="9f89c-145">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9f89c-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f89c-146">关系</span><span class="sxs-lookup"><span data-stu-id="9f89c-146">Relationships</span></span>
<span data-ttu-id="9f89c-147">无</span><span class="sxs-lookup"><span data-stu-id="9f89c-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f89c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f89c-148">JSON Representation</span></span>
<span data-ttu-id="9f89c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f89c-149">Here is a JSON representation of the resource.</span></span>
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




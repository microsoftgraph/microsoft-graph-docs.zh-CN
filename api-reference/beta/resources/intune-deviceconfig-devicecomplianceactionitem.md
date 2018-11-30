---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
ms.openlocfilehash: dc84ee71e6544bf089f3470d607772c2242f7278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043539"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="9ff20-103">deviceComplianceActionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ff20-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="9ff20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ff20-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ff20-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ff20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ff20-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ff20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ff20-107">计划的操作配置</span><span class="sxs-lookup"><span data-stu-id="9ff20-107">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="9ff20-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ff20-108">Methods</span></span>
|<span data-ttu-id="9ff20-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ff20-109">Method</span></span>|<span data-ttu-id="9ff20-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ff20-110">Return Type</span></span>|<span data-ttu-id="9ff20-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ff20-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ff20-112">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="9ff20-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="9ff20-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ff20-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="9ff20-114">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ff20-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="9ff20-115">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="9ff20-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9ff20-117">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ff20-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9ff20-118">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="9ff20-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9ff20-120">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ff20-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="9ff20-121">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="9ff20-122">无</span><span class="sxs-lookup"><span data-stu-id="9ff20-122">None</span></span>|<span data-ttu-id="9ff20-123">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9ff20-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="9ff20-124">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="9ff20-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9ff20-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="9ff20-126">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ff20-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ff20-127">属性</span><span class="sxs-lookup"><span data-stu-id="9ff20-127">Properties</span></span>
|<span data-ttu-id="9ff20-128">属性</span><span class="sxs-lookup"><span data-stu-id="9ff20-128">Property</span></span>|<span data-ttu-id="9ff20-129">类型</span><span class="sxs-lookup"><span data-stu-id="9ff20-129">Type</span></span>|<span data-ttu-id="9ff20-130">说明</span><span class="sxs-lookup"><span data-stu-id="9ff20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff20-131">id</span><span class="sxs-lookup"><span data-stu-id="9ff20-131">id</span></span>|<span data-ttu-id="9ff20-132">String</span><span class="sxs-lookup"><span data-stu-id="9ff20-132">String</span></span>|<span data-ttu-id="9ff20-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ff20-133">Key of the entity.</span></span>|
|<span data-ttu-id="9ff20-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9ff20-134">gracePeriodHours</span></span>|<span data-ttu-id="9ff20-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff20-135">Int32</span></span>|<span data-ttu-id="9ff20-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="9ff20-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9ff20-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="9ff20-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9ff20-138">actionType</span><span class="sxs-lookup"><span data-stu-id="9ff20-138">actionType</span></span>|[<span data-ttu-id="9ff20-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9ff20-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9ff20-140">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="9ff20-140">What action to take.</span></span> <span data-ttu-id="9ff20-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="9ff20-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="9ff20-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9ff20-142">notificationTemplateId</span></span>|<span data-ttu-id="9ff20-143">String</span><span class="sxs-lookup"><span data-stu-id="9ff20-143">String</span></span>|<span data-ttu-id="9ff20-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="9ff20-144">What notification Message template to use</span></span>|
|<span data-ttu-id="9ff20-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9ff20-145">notificationMessageCCList</span></span>|<span data-ttu-id="9ff20-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ff20-146">String collection</span></span>|<span data-ttu-id="9ff20-147">指定抄送此通知邮件的人员的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9ff20-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ff20-148">关系</span><span class="sxs-lookup"><span data-stu-id="9ff20-148">Relationships</span></span>
<span data-ttu-id="9ff20-149">无</span><span class="sxs-lookup"><span data-stu-id="9ff20-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ff20-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ff20-150">JSON Representation</span></span>
<span data-ttu-id="9ff20-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ff20-151">Here is a JSON representation of the resource.</span></span>
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






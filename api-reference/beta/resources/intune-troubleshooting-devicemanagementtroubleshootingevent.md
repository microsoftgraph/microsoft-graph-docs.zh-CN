---
title: deviceManagementTroubleshootingEvent 资源类型
description: 表示一般性故障的事件。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2c640ec2988be09cd19a3e87a00ebb64a3b1be3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861661"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a><span data-ttu-id="2272b-103">deviceManagementTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="2272b-103">deviceManagementTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="2272b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2272b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2272b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2272b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2272b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2272b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2272b-107">表示一般性故障的事件。</span><span class="sxs-lookup"><span data-stu-id="2272b-107">Event representing an general failure.</span></span>
## <a name="methods"></a><span data-ttu-id="2272b-108">方法</span><span class="sxs-lookup"><span data-stu-id="2272b-108">Methods</span></span>
|<span data-ttu-id="2272b-109">方法</span><span class="sxs-lookup"><span data-stu-id="2272b-109">Method</span></span>|<span data-ttu-id="2272b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2272b-110">Return Type</span></span>|<span data-ttu-id="2272b-111">说明</span><span class="sxs-lookup"><span data-stu-id="2272b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2272b-112">列出 deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="2272b-112">List deviceManagementTroubleshootingEvents</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|<span data-ttu-id="2272b-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2272b-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="2272b-114">列出 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2272b-114">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="2272b-115">获取 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-115">Get deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[<span data-ttu-id="2272b-116">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-116">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="2272b-117">读取 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2272b-117">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="2272b-118">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-118">Create deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[<span data-ttu-id="2272b-119">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-119">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="2272b-120">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2272b-120">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="2272b-121">删除 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-121">Delete deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|<span data-ttu-id="2272b-122">无</span><span class="sxs-lookup"><span data-stu-id="2272b-122">None</span></span>|<span data-ttu-id="2272b-123">删除 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="2272b-123">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="2272b-124">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-124">Update deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[<span data-ttu-id="2272b-125">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2272b-125">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="2272b-126">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2272b-126">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2272b-127">属性</span><span class="sxs-lookup"><span data-stu-id="2272b-127">Properties</span></span>
|<span data-ttu-id="2272b-128">属性</span><span class="sxs-lookup"><span data-stu-id="2272b-128">Property</span></span>|<span data-ttu-id="2272b-129">类型</span><span class="sxs-lookup"><span data-stu-id="2272b-129">Type</span></span>|<span data-ttu-id="2272b-130">说明</span><span class="sxs-lookup"><span data-stu-id="2272b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2272b-131">id</span><span class="sxs-lookup"><span data-stu-id="2272b-131">id</span></span>|<span data-ttu-id="2272b-132">String</span><span class="sxs-lookup"><span data-stu-id="2272b-132">String</span></span>|<span data-ttu-id="2272b-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="2272b-133">UUID for the object</span></span>|
|<span data-ttu-id="2272b-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="2272b-134">eventDateTime</span></span>|<span data-ttu-id="2272b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2272b-135">DateTimeOffset</span></span>|<span data-ttu-id="2272b-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="2272b-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="2272b-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="2272b-137">correlationId</span></span>|<span data-ttu-id="2272b-138">String</span><span class="sxs-lookup"><span data-stu-id="2272b-138">String</span></span>|<span data-ttu-id="2272b-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="2272b-139">Id used for tracing the failure in the service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2272b-140">关系</span><span class="sxs-lookup"><span data-stu-id="2272b-140">Relationships</span></span>
<span data-ttu-id="2272b-141">无</span><span class="sxs-lookup"><span data-stu-id="2272b-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2272b-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2272b-142">JSON Representation</span></span>
<span data-ttu-id="2272b-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2272b-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```






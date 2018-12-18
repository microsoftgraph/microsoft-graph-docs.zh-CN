---
title: deviceManagementTroubleshootingEvent 资源类型
description: 表示一般性故障的事件。
author: tfitzmac
ms.openlocfilehash: 30b77ff2ec4d1cdd6254109056b6de801743f2a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346527"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a><span data-ttu-id="f176d-103">deviceManagementTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="f176d-103">deviceManagementTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="f176d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f176d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f176d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f176d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f176d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f176d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f176d-107">表示一般性故障的事件。</span><span class="sxs-lookup"><span data-stu-id="f176d-107">Event representing an general failure.</span></span>
## <a name="methods"></a><span data-ttu-id="f176d-108">方法</span><span class="sxs-lookup"><span data-stu-id="f176d-108">Methods</span></span>
|<span data-ttu-id="f176d-109">方法</span><span class="sxs-lookup"><span data-stu-id="f176d-109">Method</span></span>|<span data-ttu-id="f176d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f176d-110">Return Type</span></span>|<span data-ttu-id="f176d-111">说明</span><span class="sxs-lookup"><span data-stu-id="f176d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f176d-112">列出 deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="f176d-112">List deviceManagementTroubleshootingEvents</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|<span data-ttu-id="f176d-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f176d-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="f176d-114">列出 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f176d-114">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="f176d-115">获取 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-115">Get deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[<span data-ttu-id="f176d-116">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-116">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="f176d-117">读取 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f176d-117">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="f176d-118">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-118">Create deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[<span data-ttu-id="f176d-119">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-119">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="f176d-120">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f176d-120">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="f176d-121">删除 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-121">Delete deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|<span data-ttu-id="f176d-122">无</span><span class="sxs-lookup"><span data-stu-id="f176d-122">None</span></span>|<span data-ttu-id="f176d-123">删除 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="f176d-123">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="f176d-124">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-124">Update deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[<span data-ttu-id="f176d-125">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f176d-125">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="f176d-126">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f176d-126">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f176d-127">属性</span><span class="sxs-lookup"><span data-stu-id="f176d-127">Properties</span></span>
|<span data-ttu-id="f176d-128">属性</span><span class="sxs-lookup"><span data-stu-id="f176d-128">Property</span></span>|<span data-ttu-id="f176d-129">类型</span><span class="sxs-lookup"><span data-stu-id="f176d-129">Type</span></span>|<span data-ttu-id="f176d-130">说明</span><span class="sxs-lookup"><span data-stu-id="f176d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f176d-131">id</span><span class="sxs-lookup"><span data-stu-id="f176d-131">id</span></span>|<span data-ttu-id="f176d-132">String</span><span class="sxs-lookup"><span data-stu-id="f176d-132">String</span></span>|<span data-ttu-id="f176d-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="f176d-133">UUID for the object</span></span>|
|<span data-ttu-id="f176d-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f176d-134">eventDateTime</span></span>|<span data-ttu-id="f176d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f176d-135">DateTimeOffset</span></span>|<span data-ttu-id="f176d-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f176d-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="f176d-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="f176d-137">correlationId</span></span>|<span data-ttu-id="f176d-138">String</span><span class="sxs-lookup"><span data-stu-id="f176d-138">String</span></span>|<span data-ttu-id="f176d-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="f176d-139">Id used for tracing the failure in the service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f176d-140">关系</span><span class="sxs-lookup"><span data-stu-id="f176d-140">Relationships</span></span>
<span data-ttu-id="f176d-141">无</span><span class="sxs-lookup"><span data-stu-id="f176d-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f176d-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f176d-142">JSON Representation</span></span>
<span data-ttu-id="f176d-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f176d-143">Here is a JSON representation of the resource.</span></span>
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






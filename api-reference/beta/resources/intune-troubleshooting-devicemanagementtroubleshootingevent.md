---
title: deviceManagementTroubleshootingEvent 资源类型
description: 表示一般性故障的事件。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a9c550b1f1285d86602aea1c8d9328869123a18f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413666"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a><span data-ttu-id="8312d-103">deviceManagementTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="8312d-103">deviceManagementTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="8312d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8312d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8312d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8312d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8312d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8312d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8312d-107">表示一般性故障的事件。</span><span class="sxs-lookup"><span data-stu-id="8312d-107">Event representing an general failure.</span></span>

## <a name="methods"></a><span data-ttu-id="8312d-108">方法</span><span class="sxs-lookup"><span data-stu-id="8312d-108">Methods</span></span>
|<span data-ttu-id="8312d-109">方法</span><span class="sxs-lookup"><span data-stu-id="8312d-109">Method</span></span>|<span data-ttu-id="8312d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8312d-110">Return Type</span></span>|<span data-ttu-id="8312d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8312d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8312d-112">列出 deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="8312d-112">List deviceManagementTroubleshootingEvents</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|<span data-ttu-id="8312d-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8312d-113">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="8312d-114">列出 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8312d-114">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="8312d-115">获取 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-115">Get deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[<span data-ttu-id="8312d-116">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-116">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="8312d-117">读取 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8312d-117">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="8312d-118">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-118">Create deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[<span data-ttu-id="8312d-119">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-119">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="8312d-120">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8312d-120">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="8312d-121">删除 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-121">Delete deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|<span data-ttu-id="8312d-122">无</span><span class="sxs-lookup"><span data-stu-id="8312d-122">None</span></span>|<span data-ttu-id="8312d-123">删除 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="8312d-123">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="8312d-124">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-124">Update deviceManagementTroubleshootingEvent</span></span>](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[<span data-ttu-id="8312d-125">deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8312d-125">deviceManagementTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|<span data-ttu-id="8312d-126">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8312d-126">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8312d-127">属性</span><span class="sxs-lookup"><span data-stu-id="8312d-127">Properties</span></span>
|<span data-ttu-id="8312d-128">属性</span><span class="sxs-lookup"><span data-stu-id="8312d-128">Property</span></span>|<span data-ttu-id="8312d-129">类型</span><span class="sxs-lookup"><span data-stu-id="8312d-129">Type</span></span>|<span data-ttu-id="8312d-130">说明</span><span class="sxs-lookup"><span data-stu-id="8312d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8312d-131">id</span><span class="sxs-lookup"><span data-stu-id="8312d-131">id</span></span>|<span data-ttu-id="8312d-132">String</span><span class="sxs-lookup"><span data-stu-id="8312d-132">String</span></span>|<span data-ttu-id="8312d-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="8312d-133">UUID for the object</span></span>|
|<span data-ttu-id="8312d-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8312d-134">eventDateTime</span></span>|<span data-ttu-id="8312d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8312d-135">DateTimeOffset</span></span>|<span data-ttu-id="8312d-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8312d-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="8312d-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="8312d-137">correlationId</span></span>|<span data-ttu-id="8312d-138">String</span><span class="sxs-lookup"><span data-stu-id="8312d-138">String</span></span>|<span data-ttu-id="8312d-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="8312d-139">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="8312d-140">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8312d-140">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="8312d-141">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8312d-141">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="8312d-142">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="8312d-142">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="8312d-143">事件名称</span><span class="sxs-lookup"><span data-stu-id="8312d-143">eventName</span></span>|<span data-ttu-id="8312d-144">String</span><span class="sxs-lookup"><span data-stu-id="8312d-144">String</span></span>|<span data-ttu-id="8312d-145">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="8312d-145">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="8312d-146">它是一个可选字段</span><span class="sxs-lookup"><span data-stu-id="8312d-146">It is an Optional field</span></span>|
|<span data-ttu-id="8312d-147">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="8312d-147">additionalInformation</span></span>|<span data-ttu-id="8312d-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8312d-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8312d-149">一组字符串键和字符串值对提供了有关疑难解答事件其他信息</span><span class="sxs-lookup"><span data-stu-id="8312d-149">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|

## <a name="relationships"></a><span data-ttu-id="8312d-150">关系</span><span class="sxs-lookup"><span data-stu-id="8312d-150">Relationships</span></span>
<span data-ttu-id="8312d-151">无</span><span class="sxs-lookup"><span data-stu-id="8312d-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8312d-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8312d-152">JSON Representation</span></span>
<span data-ttu-id="8312d-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8312d-153">Here is a JSON representation of the resource.</span></span>
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
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```





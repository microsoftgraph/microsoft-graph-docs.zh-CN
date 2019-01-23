---
title: mobileAppTroubleshootingEvent 资源类型
description: 介绍 Intune，支持多个工作流的 Microsoft Graph api mobileAppTroubleshootingEvent 资源。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb519309f68f732a28ed8f26235f01f37d9628b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429543"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="998d3-103">mobileAppTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="998d3-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="998d3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="998d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="998d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="998d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="998d3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="998d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="998d3-107">代表用户设备应用程序事件安装设备管理和故障排除事件工作流的状态。</span><span class="sxs-lookup"><span data-stu-id="998d3-107">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="998d3-108">方法</span><span class="sxs-lookup"><span data-stu-id="998d3-108">Methods</span></span>
|<span data-ttu-id="998d3-109">方法</span><span class="sxs-lookup"><span data-stu-id="998d3-109">Method</span></span>|<span data-ttu-id="998d3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="998d3-110">Return Type</span></span>|<span data-ttu-id="998d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="998d3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="998d3-112">列表 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="998d3-112">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="998d3-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)集合</span><span class="sxs-lookup"><span data-stu-id="998d3-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="998d3-114">列出属性和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="998d3-114">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="998d3-115">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-115">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="998d3-116">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-116">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="998d3-117">读取属性和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="998d3-117">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="998d3-118">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-118">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="998d3-119">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-119">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="998d3-120">创建新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="998d3-120">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="998d3-121">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-121">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="998d3-122">无</span><span class="sxs-lookup"><span data-stu-id="998d3-122">None</span></span>|<span data-ttu-id="998d3-123">删除[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="998d3-123">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="998d3-124">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-124">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="998d3-125">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="998d3-125">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="998d3-126">更新[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="998d3-126">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="998d3-127">属性</span><span class="sxs-lookup"><span data-stu-id="998d3-127">Properties</span></span>
|<span data-ttu-id="998d3-128">属性</span><span class="sxs-lookup"><span data-stu-id="998d3-128">Property</span></span>|<span data-ttu-id="998d3-129">类型</span><span class="sxs-lookup"><span data-stu-id="998d3-129">Type</span></span>|<span data-ttu-id="998d3-130">说明</span><span class="sxs-lookup"><span data-stu-id="998d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998d3-131">id</span><span class="sxs-lookup"><span data-stu-id="998d3-131">id</span></span>|<span data-ttu-id="998d3-132">String</span><span class="sxs-lookup"><span data-stu-id="998d3-132">String</span></span>|<span data-ttu-id="998d3-133">UUID 对象。</span><span class="sxs-lookup"><span data-stu-id="998d3-133">UUID for the object.</span></span>|
|<span data-ttu-id="998d3-134">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="998d3-134">**Troubleshooting**</span></span>|
|<span data-ttu-id="998d3-135">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="998d3-135">additionalInformation</span></span>|<span data-ttu-id="998d3-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="998d3-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="998d3-137">一组字符串键和字符串值对提供了有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)疑难解答事件继承其他信息</span><span class="sxs-lookup"><span data-stu-id="998d3-137">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="998d3-138">applicationId</span><span class="sxs-lookup"><span data-stu-id="998d3-138">applicationId</span></span>|<span data-ttu-id="998d3-139">String</span><span class="sxs-lookup"><span data-stu-id="998d3-139">String</span></span>|<span data-ttu-id="998d3-140">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="998d3-140">Intune application identifier.</span></span>|
|<span data-ttu-id="998d3-141">correlationId</span><span class="sxs-lookup"><span data-stu-id="998d3-141">correlationId</span></span>|<span data-ttu-id="998d3-142">String</span><span class="sxs-lookup"><span data-stu-id="998d3-142">String</span></span>|<span data-ttu-id="998d3-143">用于跟踪服务中的失败的 ID。</span><span class="sxs-lookup"><span data-stu-id="998d3-143">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="998d3-144">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="998d3-144">eventDateTime</span></span>|<span data-ttu-id="998d3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="998d3-145">DateTimeOffset</span></span>|<span data-ttu-id="998d3-146">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="998d3-146">Time when the event occurred .</span></span> |
|<span data-ttu-id="998d3-147">事件名称</span><span class="sxs-lookup"><span data-stu-id="998d3-147">eventName</span></span>|<span data-ttu-id="998d3-148">String</span><span class="sxs-lookup"><span data-stu-id="998d3-148">String</span></span>|<span data-ttu-id="998d3-149">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="998d3-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="998d3-150">可选</span><span class="sxs-lookup"><span data-stu-id="998d3-150">Optional</span></span>|
|<span data-ttu-id="998d3-151">历史记录</span><span class="sxs-lookup"><span data-stu-id="998d3-151">history</span></span>|<span data-ttu-id="998d3-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="998d3-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="998d3-153">疑难解答历史记录项 Intune 移动应用程序</span><span class="sxs-lookup"><span data-stu-id="998d3-153">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="998d3-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="998d3-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="998d3-155">String</span><span class="sxs-lookup"><span data-stu-id="998d3-155">String</span></span>|<span data-ttu-id="998d3-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="998d3-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="998d3-157">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="998d3-157">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="998d3-158">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="998d3-158">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="998d3-159">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="998d3-159">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="998d3-160">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="998d3-160">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="998d3-161">userId</span><span class="sxs-lookup"><span data-stu-id="998d3-161">userId</span></span>|<span data-ttu-id="998d3-162">String</span><span class="sxs-lookup"><span data-stu-id="998d3-162">String</span></span>|<span data-ttu-id="998d3-163">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="998d3-163">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="998d3-164">关系</span><span class="sxs-lookup"><span data-stu-id="998d3-164">Relationships</span></span>
|<span data-ttu-id="998d3-165">关系</span><span class="sxs-lookup"><span data-stu-id="998d3-165">Relationship</span></span>|<span data-ttu-id="998d3-166">类型</span><span class="sxs-lookup"><span data-stu-id="998d3-166">Type</span></span>|<span data-ttu-id="998d3-167">说明</span><span class="sxs-lookup"><span data-stu-id="998d3-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998d3-168">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="998d3-168">**Device management**</span></span>|
|<span data-ttu-id="998d3-169">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="998d3-169">appLogCollectionRequests</span></span>|<span data-ttu-id="998d3-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="998d3-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="998d3-171">AppLogUploadRequest collection 属性。</span><span class="sxs-lookup"><span data-stu-id="998d3-171">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="998d3-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="998d3-172">JSON Representation</span></span>
<span data-ttu-id="998d3-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="998d3-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
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
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





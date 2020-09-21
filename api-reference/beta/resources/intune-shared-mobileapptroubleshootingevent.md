---
title: mobileAppTroubleshootingEvent 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 资源，它支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d707b983747826a31ac35734d6f18605db7e780
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084175"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="4ffbc-103">mobileAppTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ffbc-103">mobileAppTroubleshootingEvent resource type</span></span>

<span data-ttu-id="4ffbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ffbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ffbc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ffbc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ffbc-107">表示设备管理和故障排除事件工作流的用户设备应用程序安装状态的事件。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-107">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="4ffbc-108">方法</span><span class="sxs-lookup"><span data-stu-id="4ffbc-108">Methods</span></span>
|<span data-ttu-id="4ffbc-109">方法</span><span class="sxs-lookup"><span data-stu-id="4ffbc-109">Method</span></span>|<span data-ttu-id="4ffbc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4ffbc-110">Return Type</span></span>|<span data-ttu-id="4ffbc-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ffbc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4ffbc-112">列出 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="4ffbc-112">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="4ffbc-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ffbc-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="4ffbc-114">列出 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-114">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="4ffbc-115">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-115">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="4ffbc-116">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-116">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="4ffbc-117">读取 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-117">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="4ffbc-118">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-118">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="4ffbc-119">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-119">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="4ffbc-120">创建新的 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-120">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="4ffbc-121">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-121">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="4ffbc-122">无</span><span class="sxs-lookup"><span data-stu-id="4ffbc-122">None</span></span>|<span data-ttu-id="4ffbc-123">删除 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-123">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="4ffbc-124">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-124">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="4ffbc-125">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4ffbc-125">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="4ffbc-126">更新 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-126">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ffbc-127">属性</span><span class="sxs-lookup"><span data-stu-id="4ffbc-127">Properties</span></span>
|<span data-ttu-id="4ffbc-128">属性</span><span class="sxs-lookup"><span data-stu-id="4ffbc-128">Property</span></span>|<span data-ttu-id="4ffbc-129">类型</span><span class="sxs-lookup"><span data-stu-id="4ffbc-129">Type</span></span>|<span data-ttu-id="4ffbc-130">说明</span><span class="sxs-lookup"><span data-stu-id="4ffbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ffbc-131">id</span><span class="sxs-lookup"><span data-stu-id="4ffbc-131">id</span></span>|<span data-ttu-id="4ffbc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="4ffbc-132">String</span></span>|<span data-ttu-id="4ffbc-133">对象的 UUID。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-133">UUID for the object.</span></span>|
|<span data-ttu-id="4ffbc-134">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4ffbc-134">**Troubleshooting**</span></span>|
|<span data-ttu-id="4ffbc-135">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="4ffbc-135">additionalInformation</span></span>|<span data-ttu-id="4ffbc-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ffbc-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4ffbc-137">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="4ffbc-137">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4ffbc-138">applicationId</span><span class="sxs-lookup"><span data-stu-id="4ffbc-138">applicationId</span></span>|<span data-ttu-id="4ffbc-139">String</span><span class="sxs-lookup"><span data-stu-id="4ffbc-139">String</span></span>|<span data-ttu-id="4ffbc-140">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-140">Intune application identifier.</span></span>|
|<span data-ttu-id="4ffbc-141">correlationId</span><span class="sxs-lookup"><span data-stu-id="4ffbc-141">correlationId</span></span>|<span data-ttu-id="4ffbc-142">String</span><span class="sxs-lookup"><span data-stu-id="4ffbc-142">String</span></span>|<span data-ttu-id="4ffbc-143">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-143">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="4ffbc-144">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4ffbc-144">eventDateTime</span></span>|<span data-ttu-id="4ffbc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ffbc-145">DateTimeOffset</span></span>|<span data-ttu-id="4ffbc-146">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-146">Time when the event occurred .</span></span> |
|<span data-ttu-id="4ffbc-147">名</span><span class="sxs-lookup"><span data-stu-id="4ffbc-147">eventName</span></span>|<span data-ttu-id="4ffbc-148">字符串</span><span class="sxs-lookup"><span data-stu-id="4ffbc-148">String</span></span>|<span data-ttu-id="4ffbc-149">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="4ffbc-150">可选</span><span class="sxs-lookup"><span data-stu-id="4ffbc-150">Optional</span></span>|
|<span data-ttu-id="4ffbc-151">日志</span><span class="sxs-lookup"><span data-stu-id="4ffbc-151">history</span></span>|<span data-ttu-id="4ffbc-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ffbc-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="4ffbc-153">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="4ffbc-153">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="4ffbc-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4ffbc-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="4ffbc-155">String</span><span class="sxs-lookup"><span data-stu-id="4ffbc-155">String</span></span>|<span data-ttu-id="4ffbc-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4ffbc-157">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4ffbc-157">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="4ffbc-158">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4ffbc-158">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="4ffbc-159">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-159">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="4ffbc-160">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4ffbc-160">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4ffbc-161">userId</span><span class="sxs-lookup"><span data-stu-id="4ffbc-161">userId</span></span>|<span data-ttu-id="4ffbc-162">字符串</span><span class="sxs-lookup"><span data-stu-id="4ffbc-162">String</span></span>|<span data-ttu-id="4ffbc-163">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-163">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ffbc-164">关系</span><span class="sxs-lookup"><span data-stu-id="4ffbc-164">Relationships</span></span>
|<span data-ttu-id="4ffbc-165">关系</span><span class="sxs-lookup"><span data-stu-id="4ffbc-165">Relationship</span></span>|<span data-ttu-id="4ffbc-166">类型</span><span class="sxs-lookup"><span data-stu-id="4ffbc-166">Type</span></span>|<span data-ttu-id="4ffbc-167">说明</span><span class="sxs-lookup"><span data-stu-id="4ffbc-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ffbc-168">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="4ffbc-168">**Device management**</span></span>|
|<span data-ttu-id="4ffbc-169">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="4ffbc-169">appLogCollectionRequests</span></span>|<span data-ttu-id="4ffbc-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ffbc-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="4ffbc-171">AppLogUploadRequest 的集合属性。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-171">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4ffbc-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ffbc-172">JSON Representation</span></span>
<span data-ttu-id="4ffbc-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ffbc-173">Here is a JSON representation of the resource.</span></span>
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








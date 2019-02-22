---
title: mobileAppTroubleshootingEvent 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 资源, 它支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfa126fea86c7edb302953efc3b88376f2d68a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162942"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="66ab9-103">mobileAppTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="66ab9-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="66ab9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66ab9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66ab9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66ab9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66ab9-106">表示设备管理和故障排除事件工作流的用户设备应用程序安装状态的事件。</span><span class="sxs-lookup"><span data-stu-id="66ab9-106">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="66ab9-107">方法</span><span class="sxs-lookup"><span data-stu-id="66ab9-107">Methods</span></span>
|<span data-ttu-id="66ab9-108">方法</span><span class="sxs-lookup"><span data-stu-id="66ab9-108">Method</span></span>|<span data-ttu-id="66ab9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="66ab9-109">Return Type</span></span>|<span data-ttu-id="66ab9-110">说明</span><span class="sxs-lookup"><span data-stu-id="66ab9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66ab9-111">列出 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="66ab9-111">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="66ab9-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)集合</span><span class="sxs-lookup"><span data-stu-id="66ab9-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="66ab9-113">列出[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66ab9-113">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="66ab9-114">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-114">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="66ab9-115">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-115">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="66ab9-116">读取[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66ab9-116">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="66ab9-117">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-117">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="66ab9-118">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-118">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="66ab9-119">创建新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66ab9-119">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="66ab9-120">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-120">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="66ab9-121">无</span><span class="sxs-lookup"><span data-stu-id="66ab9-121">None</span></span>|<span data-ttu-id="66ab9-122">删除[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="66ab9-122">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="66ab9-123">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-123">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="66ab9-124">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66ab9-124">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="66ab9-125">更新[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="66ab9-125">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66ab9-126">属性</span><span class="sxs-lookup"><span data-stu-id="66ab9-126">Properties</span></span>
|<span data-ttu-id="66ab9-127">属性</span><span class="sxs-lookup"><span data-stu-id="66ab9-127">Property</span></span>|<span data-ttu-id="66ab9-128">类型</span><span class="sxs-lookup"><span data-stu-id="66ab9-128">Type</span></span>|<span data-ttu-id="66ab9-129">说明</span><span class="sxs-lookup"><span data-stu-id="66ab9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66ab9-130">id</span><span class="sxs-lookup"><span data-stu-id="66ab9-130">id</span></span>|<span data-ttu-id="66ab9-131">字符串</span><span class="sxs-lookup"><span data-stu-id="66ab9-131">String</span></span>|<span data-ttu-id="66ab9-132">对象的 UUID。</span><span class="sxs-lookup"><span data-stu-id="66ab9-132">UUID for the object.</span></span>|
|<span data-ttu-id="66ab9-133">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="66ab9-133">**Troubleshooting**</span></span>|
|<span data-ttu-id="66ab9-134">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="66ab9-134">additionalInformation</span></span>|<span data-ttu-id="66ab9-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66ab9-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="66ab9-136">一组字符串键和字符串值对, 提供有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="66ab9-136">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="66ab9-137">applicationId</span><span class="sxs-lookup"><span data-stu-id="66ab9-137">applicationId</span></span>|<span data-ttu-id="66ab9-138">字符串</span><span class="sxs-lookup"><span data-stu-id="66ab9-138">String</span></span>|<span data-ttu-id="66ab9-139">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="66ab9-139">Intune application identifier.</span></span>|
|<span data-ttu-id="66ab9-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="66ab9-140">correlationId</span></span>|<span data-ttu-id="66ab9-141">String</span><span class="sxs-lookup"><span data-stu-id="66ab9-141">String</span></span>|<span data-ttu-id="66ab9-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="66ab9-142">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="66ab9-143">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="66ab9-143">eventDateTime</span></span>|<span data-ttu-id="66ab9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66ab9-144">DateTimeOffset</span></span>|<span data-ttu-id="66ab9-145">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="66ab9-145">Time when the event occurred .</span></span> |
|<span data-ttu-id="66ab9-146">名</span><span class="sxs-lookup"><span data-stu-id="66ab9-146">eventName</span></span>|<span data-ttu-id="66ab9-147">字符串</span><span class="sxs-lookup"><span data-stu-id="66ab9-147">String</span></span>|<span data-ttu-id="66ab9-148">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="66ab9-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="66ab9-149">可选</span><span class="sxs-lookup"><span data-stu-id="66ab9-149">Optional</span></span>|
|<span data-ttu-id="66ab9-150">日志</span><span class="sxs-lookup"><span data-stu-id="66ab9-150">history</span></span>|<span data-ttu-id="66ab9-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="66ab9-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="66ab9-152">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="66ab9-152">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="66ab9-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="66ab9-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="66ab9-154">String</span><span class="sxs-lookup"><span data-stu-id="66ab9-154">String</span></span>|<span data-ttu-id="66ab9-155">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="66ab9-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="66ab9-156">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="66ab9-156">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="66ab9-157">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="66ab9-157">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="66ab9-158">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="66ab9-158">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="66ab9-159">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="66ab9-159">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="66ab9-160">userId</span><span class="sxs-lookup"><span data-stu-id="66ab9-160">userId</span></span>|<span data-ttu-id="66ab9-161">String</span><span class="sxs-lookup"><span data-stu-id="66ab9-161">String</span></span>|<span data-ttu-id="66ab9-162">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="66ab9-162">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66ab9-163">关系</span><span class="sxs-lookup"><span data-stu-id="66ab9-163">Relationships</span></span>
|<span data-ttu-id="66ab9-164">关系</span><span class="sxs-lookup"><span data-stu-id="66ab9-164">Relationship</span></span>|<span data-ttu-id="66ab9-165">类型</span><span class="sxs-lookup"><span data-stu-id="66ab9-165">Type</span></span>|<span data-ttu-id="66ab9-166">说明</span><span class="sxs-lookup"><span data-stu-id="66ab9-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66ab9-167">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="66ab9-167">**Device management**</span></span>|
|<span data-ttu-id="66ab9-168">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="66ab9-168">appLogCollectionRequests</span></span>|<span data-ttu-id="66ab9-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="66ab9-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="66ab9-170">AppLogUploadRequest 的集合属性。</span><span class="sxs-lookup"><span data-stu-id="66ab9-170">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="66ab9-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66ab9-171">JSON Representation</span></span>
<span data-ttu-id="66ab9-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66ab9-172">Here is a JSON representation of the resource.</span></span>
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





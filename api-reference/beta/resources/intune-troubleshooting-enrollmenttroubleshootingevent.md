---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de3a215f83b83cfb80f83ca36da341363e5f8808
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525229"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="e0034-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0034-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="e0034-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0034-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0034-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0034-106">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="e0034-106">Event representing an enrollment failure.</span></span>


<span data-ttu-id="e0034-107">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e0034-107">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e0034-108">方法</span><span class="sxs-lookup"><span data-stu-id="e0034-108">Methods</span></span>
|<span data-ttu-id="e0034-109">方法</span><span class="sxs-lookup"><span data-stu-id="e0034-109">Method</span></span>|<span data-ttu-id="e0034-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0034-110">Return Type</span></span>|<span data-ttu-id="e0034-111">说明</span><span class="sxs-lookup"><span data-stu-id="e0034-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0034-112">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="e0034-112">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="e0034-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0034-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="e0034-114">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0034-114">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="e0034-115">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-115">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="e0034-116">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-116">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="e0034-117">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0034-117">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="e0034-118">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-118">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="e0034-119">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-119">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="e0034-120">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0034-120">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="e0034-121">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-121">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="e0034-122">无</span><span class="sxs-lookup"><span data-stu-id="e0034-122">None</span></span>|<span data-ttu-id="e0034-123">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="e0034-123">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="e0034-124">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-124">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="e0034-125">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e0034-125">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="e0034-126">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0034-126">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0034-127">属性</span><span class="sxs-lookup"><span data-stu-id="e0034-127">Properties</span></span>
|<span data-ttu-id="e0034-128">属性</span><span class="sxs-lookup"><span data-stu-id="e0034-128">Property</span></span>|<span data-ttu-id="e0034-129">类型</span><span class="sxs-lookup"><span data-stu-id="e0034-129">Type</span></span>|<span data-ttu-id="e0034-130">说明</span><span class="sxs-lookup"><span data-stu-id="e0034-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0034-131">id</span><span class="sxs-lookup"><span data-stu-id="e0034-131">id</span></span>|<span data-ttu-id="e0034-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-132">String</span></span>|<span data-ttu-id="e0034-133">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e0034-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e0034-134">eventDateTime</span></span>|<span data-ttu-id="e0034-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0034-135">DateTimeOffset</span></span>|<span data-ttu-id="e0034-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e0034-136">Time when the event occurred .</span></span> <span data-ttu-id="e0034-137">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e0034-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="e0034-138">correlationId</span></span>|<span data-ttu-id="e0034-139">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-139">String</span></span>|<span data-ttu-id="e0034-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="e0034-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e0034-141">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e0034-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e0034-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e0034-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e0034-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e0034-144">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="e0034-144">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="e0034-145">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e0034-145">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-146">名</span><span class="sxs-lookup"><span data-stu-id="e0034-146">eventName</span></span>|<span data-ttu-id="e0034-147">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-147">String</span></span>|<span data-ttu-id="e0034-148">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="e0034-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e0034-149">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="e0034-149">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-150">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e0034-150">additionalInformation</span></span>|<span data-ttu-id="e0034-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0034-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e0034-152">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="e0034-152">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e0034-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0034-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="e0034-154">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-154">String</span></span>|<span data-ttu-id="e0034-155">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="e0034-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e0034-156">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0034-156">operatingSystem</span></span>|<span data-ttu-id="e0034-157">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-157">String</span></span>|<span data-ttu-id="e0034-158">操作系统。</span><span class="sxs-lookup"><span data-stu-id="e0034-158">Operating System.</span></span>|
|<span data-ttu-id="e0034-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="e0034-159">osVersion</span></span>|<span data-ttu-id="e0034-160">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-160">String</span></span>|<span data-ttu-id="e0034-161">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e0034-161">OS Version.</span></span>|
|<span data-ttu-id="e0034-162">userId</span><span class="sxs-lookup"><span data-stu-id="e0034-162">userId</span></span>|<span data-ttu-id="e0034-163">String</span><span class="sxs-lookup"><span data-stu-id="e0034-163">String</span></span>|<span data-ttu-id="e0034-164">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="e0034-164">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e0034-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="e0034-165">deviceId</span></span>|<span data-ttu-id="e0034-166">字符串</span><span class="sxs-lookup"><span data-stu-id="e0034-166">String</span></span>|<span data-ttu-id="e0034-167">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="e0034-167">Azure AD device identifier.</span></span>|
|<span data-ttu-id="e0034-168">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="e0034-168">enrollmentType</span></span>|[<span data-ttu-id="e0034-169">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e0034-169">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="e0034-170">注册类型。</span><span class="sxs-lookup"><span data-stu-id="e0034-170">Type of the enrollment.</span></span> <span data-ttu-id="e0034-171">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="e0034-171">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="e0034-172">failureCategory</span><span class="sxs-lookup"><span data-stu-id="e0034-172">failureCategory</span></span>|[<span data-ttu-id="e0034-173">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e0034-173">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="e0034-174">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="e0034-174">Highlevel failure category.</span></span> <span data-ttu-id="e0034-175">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="e0034-175">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="e0034-176">failureReason</span><span class="sxs-lookup"><span data-stu-id="e0034-176">failureReason</span></span>|<span data-ttu-id="e0034-177">String</span><span class="sxs-lookup"><span data-stu-id="e0034-177">String</span></span>|<span data-ttu-id="e0034-178">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="e0034-178">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0034-179">关系</span><span class="sxs-lookup"><span data-stu-id="e0034-179">Relationships</span></span>
<span data-ttu-id="e0034-180">无</span><span class="sxs-lookup"><span data-stu-id="e0034-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0034-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0034-181">JSON Representation</span></span>
<span data-ttu-id="e0034-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0034-182">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
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
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```




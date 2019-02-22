---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b2f18bab64949b445aa0a5e9814675fca45377c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148291"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="c18db-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c18db-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="c18db-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c18db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c18db-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c18db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18db-106">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="c18db-106">Event representing an enrollment failure.</span></span>


<span data-ttu-id="c18db-107">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c18db-107">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c18db-108">方法</span><span class="sxs-lookup"><span data-stu-id="c18db-108">Methods</span></span>
|<span data-ttu-id="c18db-109">方法</span><span class="sxs-lookup"><span data-stu-id="c18db-109">Method</span></span>|<span data-ttu-id="c18db-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c18db-110">Return Type</span></span>|<span data-ttu-id="c18db-111">说明</span><span class="sxs-lookup"><span data-stu-id="c18db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c18db-112">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c18db-112">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="c18db-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c18db-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c18db-114">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c18db-114">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="c18db-115">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-115">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="c18db-116">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-116">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c18db-117">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c18db-117">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c18db-118">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-118">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="c18db-119">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-119">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c18db-120">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c18db-120">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c18db-121">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-121">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="c18db-122">无</span><span class="sxs-lookup"><span data-stu-id="c18db-122">None</span></span>|<span data-ttu-id="c18db-123">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="c18db-123">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="c18db-124">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-124">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="c18db-125">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c18db-125">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c18db-126">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c18db-126">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c18db-127">属性</span><span class="sxs-lookup"><span data-stu-id="c18db-127">Properties</span></span>
|<span data-ttu-id="c18db-128">属性</span><span class="sxs-lookup"><span data-stu-id="c18db-128">Property</span></span>|<span data-ttu-id="c18db-129">类型</span><span class="sxs-lookup"><span data-stu-id="c18db-129">Type</span></span>|<span data-ttu-id="c18db-130">说明</span><span class="sxs-lookup"><span data-stu-id="c18db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18db-131">id</span><span class="sxs-lookup"><span data-stu-id="c18db-131">id</span></span>|<span data-ttu-id="c18db-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-132">String</span></span>|<span data-ttu-id="c18db-133">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c18db-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c18db-134">eventDateTime</span></span>|<span data-ttu-id="c18db-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c18db-135">DateTimeOffset</span></span>|<span data-ttu-id="c18db-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c18db-136">Time when the event occurred .</span></span> <span data-ttu-id="c18db-137">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c18db-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="c18db-138">correlationId</span></span>|<span data-ttu-id="c18db-139">String</span><span class="sxs-lookup"><span data-stu-id="c18db-139">String</span></span>|<span data-ttu-id="c18db-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="c18db-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c18db-141">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c18db-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c18db-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c18db-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c18db-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c18db-144">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="c18db-144">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c18db-145">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c18db-145">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-146">名</span><span class="sxs-lookup"><span data-stu-id="c18db-146">eventName</span></span>|<span data-ttu-id="c18db-147">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-147">String</span></span>|<span data-ttu-id="c18db-148">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="c18db-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c18db-149">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="c18db-149">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-150">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="c18db-150">additionalInformation</span></span>|<span data-ttu-id="c18db-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c18db-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c18db-152">一组字符串键和字符串值对, 提供有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="c18db-152">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c18db-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c18db-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="c18db-154">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-154">String</span></span>|<span data-ttu-id="c18db-155">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c18db-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c18db-156">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c18db-156">operatingSystem</span></span>|<span data-ttu-id="c18db-157">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-157">String</span></span>|<span data-ttu-id="c18db-158">操作系统。</span><span class="sxs-lookup"><span data-stu-id="c18db-158">Operating System.</span></span>|
|<span data-ttu-id="c18db-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="c18db-159">osVersion</span></span>|<span data-ttu-id="c18db-160">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-160">String</span></span>|<span data-ttu-id="c18db-161">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c18db-161">OS Version.</span></span>|
|<span data-ttu-id="c18db-162">userId</span><span class="sxs-lookup"><span data-stu-id="c18db-162">userId</span></span>|<span data-ttu-id="c18db-163">String</span><span class="sxs-lookup"><span data-stu-id="c18db-163">String</span></span>|<span data-ttu-id="c18db-164">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="c18db-164">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c18db-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="c18db-165">deviceId</span></span>|<span data-ttu-id="c18db-166">字符串</span><span class="sxs-lookup"><span data-stu-id="c18db-166">String</span></span>|<span data-ttu-id="c18db-167">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c18db-167">Azure AD device identifier.</span></span>|
|<span data-ttu-id="c18db-168">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c18db-168">enrollmentType</span></span>|[<span data-ttu-id="c18db-169">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c18db-169">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c18db-170">注册类型。</span><span class="sxs-lookup"><span data-stu-id="c18db-170">Type of the enrollment.</span></span> <span data-ttu-id="c18db-171">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="c18db-171">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="c18db-172">failureCategory</span><span class="sxs-lookup"><span data-stu-id="c18db-172">failureCategory</span></span>|[<span data-ttu-id="c18db-173">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="c18db-173">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="c18db-174">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="c18db-174">Highlevel failure category.</span></span> <span data-ttu-id="c18db-175">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="c18db-175">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="c18db-176">failureReason</span><span class="sxs-lookup"><span data-stu-id="c18db-176">failureReason</span></span>|<span data-ttu-id="c18db-177">String</span><span class="sxs-lookup"><span data-stu-id="c18db-177">String</span></span>|<span data-ttu-id="c18db-178">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="c18db-178">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c18db-179">关系</span><span class="sxs-lookup"><span data-stu-id="c18db-179">Relationships</span></span>
<span data-ttu-id="c18db-180">无</span><span class="sxs-lookup"><span data-stu-id="c18db-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c18db-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c18db-181">JSON Representation</span></span>
<span data-ttu-id="c18db-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c18db-182">Here is a JSON representation of the resource.</span></span>
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





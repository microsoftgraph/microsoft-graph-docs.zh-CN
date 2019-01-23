---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e96e2e28117317309d2a60d9d0d780da50a718a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395928"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="b941f-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b941f-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="b941f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b941f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b941f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b941f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b941f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b941f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b941f-107">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="b941f-107">Event representing an enrollment failure.</span></span>


<span data-ttu-id="b941f-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b941f-109">方法</span><span class="sxs-lookup"><span data-stu-id="b941f-109">Methods</span></span>
|<span data-ttu-id="b941f-110">方法</span><span class="sxs-lookup"><span data-stu-id="b941f-110">Method</span></span>|<span data-ttu-id="b941f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b941f-111">Return Type</span></span>|<span data-ttu-id="b941f-112">说明</span><span class="sxs-lookup"><span data-stu-id="b941f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b941f-113">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="b941f-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="b941f-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b941f-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="b941f-115">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b941f-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="b941f-116">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="b941f-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b941f-118">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b941f-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="b941f-119">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="b941f-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b941f-121">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b941f-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="b941f-122">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="b941f-123">无</span><span class="sxs-lookup"><span data-stu-id="b941f-123">None</span></span>|<span data-ttu-id="b941f-124">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="b941f-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="b941f-125">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="b941f-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b941f-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b941f-127">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b941f-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b941f-128">属性</span><span class="sxs-lookup"><span data-stu-id="b941f-128">Properties</span></span>
|<span data-ttu-id="b941f-129">属性</span><span class="sxs-lookup"><span data-stu-id="b941f-129">Property</span></span>|<span data-ttu-id="b941f-130">类型</span><span class="sxs-lookup"><span data-stu-id="b941f-130">Type</span></span>|<span data-ttu-id="b941f-131">说明</span><span class="sxs-lookup"><span data-stu-id="b941f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b941f-132">id</span><span class="sxs-lookup"><span data-stu-id="b941f-132">id</span></span>|<span data-ttu-id="b941f-133">String</span><span class="sxs-lookup"><span data-stu-id="b941f-133">String</span></span>|<span data-ttu-id="b941f-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b941f-135">eventDateTime</span></span>|<span data-ttu-id="b941f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b941f-136">DateTimeOffset</span></span>|<span data-ttu-id="b941f-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b941f-137">Time when the event occurred .</span></span> <span data-ttu-id="b941f-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="b941f-139">correlationId</span></span>|<span data-ttu-id="b941f-140">String</span><span class="sxs-lookup"><span data-stu-id="b941f-140">String</span></span>|<span data-ttu-id="b941f-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="b941f-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b941f-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b941f-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b941f-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b941f-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b941f-145">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="b941f-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="b941f-146">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-147">事件名称</span><span class="sxs-lookup"><span data-stu-id="b941f-147">eventName</span></span>|<span data-ttu-id="b941f-148">String</span><span class="sxs-lookup"><span data-stu-id="b941f-148">String</span></span>|<span data-ttu-id="b941f-149">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="b941f-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="b941f-150">它是一个可选字段继承从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b941f-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="b941f-151">additionalInformation</span></span>|<span data-ttu-id="b941f-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b941f-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b941f-153">一组字符串键和字符串值对提供了有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)疑难解答事件继承其他信息</span><span class="sxs-lookup"><span data-stu-id="b941f-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b941f-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b941f-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="b941f-155">String</span><span class="sxs-lookup"><span data-stu-id="b941f-155">String</span></span>|<span data-ttu-id="b941f-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="b941f-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b941f-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b941f-157">operatingSystem</span></span>|<span data-ttu-id="b941f-158">String</span><span class="sxs-lookup"><span data-stu-id="b941f-158">String</span></span>|<span data-ttu-id="b941f-159">操作系统。</span><span class="sxs-lookup"><span data-stu-id="b941f-159">Operating System.</span></span>|
|<span data-ttu-id="b941f-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="b941f-160">osVersion</span></span>|<span data-ttu-id="b941f-161">String</span><span class="sxs-lookup"><span data-stu-id="b941f-161">String</span></span>|<span data-ttu-id="b941f-162">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b941f-162">OS Version.</span></span>|
|<span data-ttu-id="b941f-163">userId</span><span class="sxs-lookup"><span data-stu-id="b941f-163">userId</span></span>|<span data-ttu-id="b941f-164">String</span><span class="sxs-lookup"><span data-stu-id="b941f-164">String</span></span>|<span data-ttu-id="b941f-165">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="b941f-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b941f-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="b941f-166">deviceId</span></span>|<span data-ttu-id="b941f-167">String</span><span class="sxs-lookup"><span data-stu-id="b941f-167">String</span></span>|<span data-ttu-id="b941f-168">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="b941f-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b941f-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b941f-169">enrollmentType</span></span>|[<span data-ttu-id="b941f-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b941f-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b941f-171">注册类型。</span><span class="sxs-lookup"><span data-stu-id="b941f-171">Type of the enrollment.</span></span> <span data-ttu-id="b941f-172">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="b941f-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b941f-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b941f-173">failureCategory</span></span>|[<span data-ttu-id="b941f-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="b941f-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="b941f-175">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="b941f-175">Highlevel failure category.</span></span> <span data-ttu-id="b941f-176">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="b941f-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b941f-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="b941f-177">failureReason</span></span>|<span data-ttu-id="b941f-178">String</span><span class="sxs-lookup"><span data-stu-id="b941f-178">String</span></span>|<span data-ttu-id="b941f-179">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="b941f-179">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b941f-180">关系</span><span class="sxs-lookup"><span data-stu-id="b941f-180">Relationships</span></span>
<span data-ttu-id="b941f-181">无</span><span class="sxs-lookup"><span data-stu-id="b941f-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b941f-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b941f-182">JSON Representation</span></span>
<span data-ttu-id="b941f-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b941f-183">Here is a JSON representation of the resource.</span></span>
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





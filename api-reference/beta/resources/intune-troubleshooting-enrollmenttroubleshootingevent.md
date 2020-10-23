---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 170095b1675c61004dcd6a2c0a1d644b73ac098d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730330"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="597fc-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="597fc-103">enrollmentTroubleshootingEvent resource type</span></span>

<span data-ttu-id="597fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="597fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="597fc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="597fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="597fc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="597fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="597fc-107">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="597fc-107">Event representing an enrollment failure.</span></span>


<span data-ttu-id="597fc-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="597fc-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="597fc-109">Methods</span><span class="sxs-lookup"><span data-stu-id="597fc-109">Methods</span></span>
|<span data-ttu-id="597fc-110">方法</span><span class="sxs-lookup"><span data-stu-id="597fc-110">Method</span></span>|<span data-ttu-id="597fc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="597fc-111">Return Type</span></span>|<span data-ttu-id="597fc-112">说明</span><span class="sxs-lookup"><span data-stu-id="597fc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="597fc-113">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="597fc-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="597fc-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="597fc-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="597fc-115">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="597fc-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="597fc-116">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="597fc-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="597fc-118">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="597fc-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="597fc-119">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="597fc-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="597fc-121">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="597fc-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="597fc-122">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="597fc-123">无</span><span class="sxs-lookup"><span data-stu-id="597fc-123">None</span></span>|<span data-ttu-id="597fc-124">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="597fc-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="597fc-125">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="597fc-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="597fc-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="597fc-127">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="597fc-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="597fc-128">属性</span><span class="sxs-lookup"><span data-stu-id="597fc-128">Properties</span></span>
|<span data-ttu-id="597fc-129">属性</span><span class="sxs-lookup"><span data-stu-id="597fc-129">Property</span></span>|<span data-ttu-id="597fc-130">类型</span><span class="sxs-lookup"><span data-stu-id="597fc-130">Type</span></span>|<span data-ttu-id="597fc-131">说明</span><span class="sxs-lookup"><span data-stu-id="597fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="597fc-132">id</span><span class="sxs-lookup"><span data-stu-id="597fc-132">id</span></span>|<span data-ttu-id="597fc-133">String</span><span class="sxs-lookup"><span data-stu-id="597fc-133">String</span></span>|<span data-ttu-id="597fc-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="597fc-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="597fc-135">eventDateTime</span></span>|<span data-ttu-id="597fc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="597fc-136">DateTimeOffset</span></span>|<span data-ttu-id="597fc-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="597fc-137">Time when the event occurred .</span></span> <span data-ttu-id="597fc-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="597fc-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="597fc-139">correlationId</span></span>|<span data-ttu-id="597fc-140">String</span><span class="sxs-lookup"><span data-stu-id="597fc-140">String</span></span>|<span data-ttu-id="597fc-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="597fc-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="597fc-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="597fc-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="597fc-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="597fc-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="597fc-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="597fc-145">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="597fc-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="597fc-146">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="597fc-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-147">名</span><span class="sxs-lookup"><span data-stu-id="597fc-147">eventName</span></span>|<span data-ttu-id="597fc-148">String</span><span class="sxs-lookup"><span data-stu-id="597fc-148">String</span></span>|<span data-ttu-id="597fc-149">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="597fc-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="597fc-150">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="597fc-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="597fc-151">additionalInformation</span></span>|<span data-ttu-id="597fc-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="597fc-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="597fc-153">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="597fc-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="597fc-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="597fc-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="597fc-155">String</span><span class="sxs-lookup"><span data-stu-id="597fc-155">String</span></span>|<span data-ttu-id="597fc-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="597fc-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="597fc-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="597fc-157">operatingSystem</span></span>|<span data-ttu-id="597fc-158">String</span><span class="sxs-lookup"><span data-stu-id="597fc-158">String</span></span>|<span data-ttu-id="597fc-159">操作系统。</span><span class="sxs-lookup"><span data-stu-id="597fc-159">Operating System.</span></span>|
|<span data-ttu-id="597fc-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="597fc-160">osVersion</span></span>|<span data-ttu-id="597fc-161">String</span><span class="sxs-lookup"><span data-stu-id="597fc-161">String</span></span>|<span data-ttu-id="597fc-162">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="597fc-162">OS Version.</span></span>|
|<span data-ttu-id="597fc-163">userId</span><span class="sxs-lookup"><span data-stu-id="597fc-163">userId</span></span>|<span data-ttu-id="597fc-164">String</span><span class="sxs-lookup"><span data-stu-id="597fc-164">String</span></span>|<span data-ttu-id="597fc-165">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="597fc-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="597fc-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="597fc-166">deviceId</span></span>|<span data-ttu-id="597fc-167">String</span><span class="sxs-lookup"><span data-stu-id="597fc-167">String</span></span>|<span data-ttu-id="597fc-168">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="597fc-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="597fc-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="597fc-169">enrollmentType</span></span>|[<span data-ttu-id="597fc-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="597fc-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="597fc-171">注册类型。</span><span class="sxs-lookup"><span data-stu-id="597fc-171">Type of the enrollment.</span></span> <span data-ttu-id="597fc-172">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="597fc-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="597fc-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="597fc-173">failureCategory</span></span>|[<span data-ttu-id="597fc-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="597fc-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="597fc-175">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="597fc-175">Highlevel failure category.</span></span> <span data-ttu-id="597fc-176">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="597fc-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="597fc-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="597fc-177">failureReason</span></span>|<span data-ttu-id="597fc-178">String</span><span class="sxs-lookup"><span data-stu-id="597fc-178">String</span></span>|<span data-ttu-id="597fc-179">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="597fc-179">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="597fc-180">关系</span><span class="sxs-lookup"><span data-stu-id="597fc-180">Relationships</span></span>
<span data-ttu-id="597fc-181">无</span><span class="sxs-lookup"><span data-stu-id="597fc-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="597fc-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="597fc-182">JSON Representation</span></span>
<span data-ttu-id="597fc-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="597fc-183">Here is a JSON representation of the resource.</span></span>
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






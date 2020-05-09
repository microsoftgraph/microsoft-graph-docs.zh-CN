---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b1047eb10dc33ff178308a9b31d6d959a966bedc
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177651"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="3275d-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="3275d-103">enrollmentTroubleshootingEvent resource type</span></span>

<span data-ttu-id="3275d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3275d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3275d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3275d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3275d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3275d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3275d-107">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="3275d-107">Event representing an enrollment failure.</span></span>


<span data-ttu-id="3275d-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3275d-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3275d-109">方法</span><span class="sxs-lookup"><span data-stu-id="3275d-109">Methods</span></span>
|<span data-ttu-id="3275d-110">方法</span><span class="sxs-lookup"><span data-stu-id="3275d-110">Method</span></span>|<span data-ttu-id="3275d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3275d-111">Return Type</span></span>|<span data-ttu-id="3275d-112">说明</span><span class="sxs-lookup"><span data-stu-id="3275d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3275d-113">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="3275d-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="3275d-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3275d-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="3275d-115">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3275d-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="3275d-116">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="3275d-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="3275d-118">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3275d-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="3275d-119">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="3275d-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="3275d-121">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3275d-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="3275d-122">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="3275d-123">无</span><span class="sxs-lookup"><span data-stu-id="3275d-123">None</span></span>|<span data-ttu-id="3275d-124">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="3275d-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="3275d-125">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="3275d-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3275d-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="3275d-127">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3275d-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3275d-128">属性</span><span class="sxs-lookup"><span data-stu-id="3275d-128">Properties</span></span>
|<span data-ttu-id="3275d-129">属性</span><span class="sxs-lookup"><span data-stu-id="3275d-129">Property</span></span>|<span data-ttu-id="3275d-130">类型</span><span class="sxs-lookup"><span data-stu-id="3275d-130">Type</span></span>|<span data-ttu-id="3275d-131">说明</span><span class="sxs-lookup"><span data-stu-id="3275d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3275d-132">id</span><span class="sxs-lookup"><span data-stu-id="3275d-132">id</span></span>|<span data-ttu-id="3275d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-133">String</span></span>|<span data-ttu-id="3275d-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3275d-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3275d-135">eventDateTime</span></span>|<span data-ttu-id="3275d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3275d-136">DateTimeOffset</span></span>|<span data-ttu-id="3275d-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="3275d-137">Time when the event occurred .</span></span> <span data-ttu-id="3275d-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3275d-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="3275d-139">correlationId</span></span>|<span data-ttu-id="3275d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-140">String</span></span>|<span data-ttu-id="3275d-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="3275d-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="3275d-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3275d-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3275d-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3275d-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3275d-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3275d-145">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="3275d-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3275d-146">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3275d-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-147">名</span><span class="sxs-lookup"><span data-stu-id="3275d-147">eventName</span></span>|<span data-ttu-id="3275d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-148">String</span></span>|<span data-ttu-id="3275d-149">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="3275d-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="3275d-150">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="3275d-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="3275d-151">additionalInformation</span></span>|<span data-ttu-id="3275d-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3275d-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3275d-153">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="3275d-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3275d-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3275d-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="3275d-155">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-155">String</span></span>|<span data-ttu-id="3275d-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3275d-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3275d-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3275d-157">operatingSystem</span></span>|<span data-ttu-id="3275d-158">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-158">String</span></span>|<span data-ttu-id="3275d-159">操作系统。</span><span class="sxs-lookup"><span data-stu-id="3275d-159">Operating System.</span></span>|
|<span data-ttu-id="3275d-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="3275d-160">osVersion</span></span>|<span data-ttu-id="3275d-161">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-161">String</span></span>|<span data-ttu-id="3275d-162">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3275d-162">OS Version.</span></span>|
|<span data-ttu-id="3275d-163">userId</span><span class="sxs-lookup"><span data-stu-id="3275d-163">userId</span></span>|<span data-ttu-id="3275d-164">String</span><span class="sxs-lookup"><span data-stu-id="3275d-164">String</span></span>|<span data-ttu-id="3275d-165">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="3275d-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="3275d-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="3275d-166">deviceId</span></span>|<span data-ttu-id="3275d-167">字符串</span><span class="sxs-lookup"><span data-stu-id="3275d-167">String</span></span>|<span data-ttu-id="3275d-168">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3275d-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="3275d-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="3275d-169">enrollmentType</span></span>|[<span data-ttu-id="3275d-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3275d-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3275d-171">注册类型。</span><span class="sxs-lookup"><span data-stu-id="3275d-171">Type of the enrollment.</span></span> <span data-ttu-id="3275d-172">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="3275d-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="3275d-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="3275d-173">failureCategory</span></span>|[<span data-ttu-id="3275d-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="3275d-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="3275d-175">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="3275d-175">Highlevel failure category.</span></span> <span data-ttu-id="3275d-176">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="3275d-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="3275d-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="3275d-177">failureReason</span></span>|<span data-ttu-id="3275d-178">String</span><span class="sxs-lookup"><span data-stu-id="3275d-178">String</span></span>|<span data-ttu-id="3275d-179">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="3275d-179">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3275d-180">关系</span><span class="sxs-lookup"><span data-stu-id="3275d-180">Relationships</span></span>
<span data-ttu-id="3275d-181">无</span><span class="sxs-lookup"><span data-stu-id="3275d-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3275d-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3275d-182">JSON Representation</span></span>
<span data-ttu-id="3275d-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3275d-183">Here is a JSON representation of the resource.</span></span>
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




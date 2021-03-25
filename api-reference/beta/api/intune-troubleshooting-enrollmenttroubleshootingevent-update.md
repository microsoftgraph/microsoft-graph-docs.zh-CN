---
title: 更新 enrollmentTroubleshootingEvent
description: 更新 enrollmentTroubleshootingEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac5fa06e43a83a6c8de58e1b79faa8f78a50172f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151898"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="7bfd7-103">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7bfd7-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="7bfd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bfd7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bfd7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bfd7-107">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bfd7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bfd7-108">Prerequisites</span></span>
<span data-ttu-id="7bfd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bfd7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bfd7-111">Permission type</span></span>|<span data-ttu-id="7bfd7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bfd7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bfd7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bfd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bfd7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bfd7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7bfd7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bfd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bfd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-116">Not supported.</span></span>|
|<span data-ttu-id="7bfd7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bfd7-117">Application</span></span>|<span data-ttu-id="7bfd7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bfd7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bfd7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bfd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7bfd7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bfd7-120">Request headers</span></span>
|<span data-ttu-id="7bfd7-121">标头</span><span class="sxs-lookup"><span data-stu-id="7bfd7-121">Header</span></span>|<span data-ttu-id="7bfd7-122">值</span><span class="sxs-lookup"><span data-stu-id="7bfd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bfd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bfd7-123">Authorization</span></span>|<span data-ttu-id="7bfd7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bfd7-125">接受</span><span class="sxs-lookup"><span data-stu-id="7bfd7-125">Accept</span></span>|<span data-ttu-id="7bfd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bfd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bfd7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bfd7-127">Request body</span></span>
<span data-ttu-id="7bfd7-128">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="7bfd7-129">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="7bfd7-130">属性</span><span class="sxs-lookup"><span data-stu-id="7bfd7-130">Property</span></span>|<span data-ttu-id="7bfd7-131">类型</span><span class="sxs-lookup"><span data-stu-id="7bfd7-131">Type</span></span>|<span data-ttu-id="7bfd7-132">说明</span><span class="sxs-lookup"><span data-stu-id="7bfd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bfd7-133">id</span><span class="sxs-lookup"><span data-stu-id="7bfd7-133">id</span></span>|<span data-ttu-id="7bfd7-134">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-134">String</span></span>|<span data-ttu-id="7bfd7-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7bfd7-136">eventDateTime</span></span>|<span data-ttu-id="7bfd7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bfd7-137">DateTimeOffset</span></span>|<span data-ttu-id="7bfd7-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-138">Time when the event occurred .</span></span> <span data-ttu-id="7bfd7-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="7bfd7-140">correlationId</span></span>|<span data-ttu-id="7bfd7-141">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-141">String</span></span>|<span data-ttu-id="7bfd7-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="7bfd7-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7bfd7-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="7bfd7-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7bfd7-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="7bfd7-146">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="7bfd7-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-148">eventName</span><span class="sxs-lookup"><span data-stu-id="7bfd7-148">eventName</span></span>|<span data-ttu-id="7bfd7-149">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-149">String</span></span>|<span data-ttu-id="7bfd7-150">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="7bfd7-151">它是可选字段 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="7bfd7-152">additionalInformation</span></span>|<span data-ttu-id="7bfd7-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7bfd7-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7bfd7-154">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7bfd7-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7bfd7-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7bfd7-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="7bfd7-156">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-156">String</span></span>|<span data-ttu-id="7bfd7-157">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="7bfd7-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7bfd7-158">operatingSystem</span></span>|<span data-ttu-id="7bfd7-159">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-159">String</span></span>|<span data-ttu-id="7bfd7-160">操作系统。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-160">Operating System.</span></span>|
|<span data-ttu-id="7bfd7-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="7bfd7-161">osVersion</span></span>|<span data-ttu-id="7bfd7-162">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-162">String</span></span>|<span data-ttu-id="7bfd7-163">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-163">OS Version.</span></span>|
|<span data-ttu-id="7bfd7-164">userId</span><span class="sxs-lookup"><span data-stu-id="7bfd7-164">userId</span></span>|<span data-ttu-id="7bfd7-165">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-165">String</span></span>|<span data-ttu-id="7bfd7-166">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="7bfd7-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="7bfd7-167">deviceId</span></span>|<span data-ttu-id="7bfd7-168">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-168">String</span></span>|<span data-ttu-id="7bfd7-169">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="7bfd7-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="7bfd7-170">enrollmentType</span></span>|[<span data-ttu-id="7bfd7-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7bfd7-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="7bfd7-172">注册类型。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-172">Type of the enrollment.</span></span> <span data-ttu-id="7bfd7-173">可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="7bfd7-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="7bfd7-174">failureCategory</span></span>|[<span data-ttu-id="7bfd7-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="7bfd7-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="7bfd7-176">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-176">Highlevel failure category.</span></span> <span data-ttu-id="7bfd7-177">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="7bfd7-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="7bfd7-178">failureReason</span></span>|<span data-ttu-id="7bfd7-179">String</span><span class="sxs-lookup"><span data-stu-id="7bfd7-179">String</span></span>|<span data-ttu-id="7bfd7-180">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="7bfd7-181">响应</span><span class="sxs-lookup"><span data-stu-id="7bfd7-181">Response</span></span>
<span data-ttu-id="7bfd7-182">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bfd7-183">示例</span><span class="sxs-lookup"><span data-stu-id="7bfd7-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bfd7-184">请求</span><span class="sxs-lookup"><span data-stu-id="7bfd7-184">Request</span></span>
<span data-ttu-id="7bfd7-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="7bfd7-186">响应</span><span class="sxs-lookup"><span data-stu-id="7bfd7-186">Response</span></span>
<span data-ttu-id="7bfd7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bfd7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1231

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```





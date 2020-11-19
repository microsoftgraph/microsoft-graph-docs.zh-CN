---
title: 更新 enrollmentTroubleshootingEvent
description: 更新 enrollmentTroubleshootingEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58273ba4e42bd3ed27e35fd3eee16321202eb416
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223337"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="00a2a-103">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="00a2a-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="00a2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00a2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00a2a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00a2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00a2a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00a2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a2a-107">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00a2a-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00a2a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="00a2a-108">Prerequisites</span></span>
<span data-ttu-id="00a2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="00a2a-111">Permission type</span></span>|<span data-ttu-id="00a2a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00a2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00a2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00a2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00a2a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a2a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="00a2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00a2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00a2a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="00a2a-116">Not supported.</span></span>|
|<span data-ttu-id="00a2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="00a2a-117">Application</span></span>|<span data-ttu-id="00a2a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a2a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00a2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00a2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="00a2a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="00a2a-120">Request headers</span></span>
|<span data-ttu-id="00a2a-121">标头</span><span class="sxs-lookup"><span data-stu-id="00a2a-121">Header</span></span>|<span data-ttu-id="00a2a-122">值</span><span class="sxs-lookup"><span data-stu-id="00a2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00a2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00a2a-123">Authorization</span></span>|<span data-ttu-id="00a2a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00a2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00a2a-125">接受</span><span class="sxs-lookup"><span data-stu-id="00a2a-125">Accept</span></span>|<span data-ttu-id="00a2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00a2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00a2a-127">Request body</span></span>
<span data-ttu-id="00a2a-128">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00a2a-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="00a2a-129">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00a2a-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="00a2a-130">属性</span><span class="sxs-lookup"><span data-stu-id="00a2a-130">Property</span></span>|<span data-ttu-id="00a2a-131">类型</span><span class="sxs-lookup"><span data-stu-id="00a2a-131">Type</span></span>|<span data-ttu-id="00a2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="00a2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a2a-133">id</span><span class="sxs-lookup"><span data-stu-id="00a2a-133">id</span></span>|<span data-ttu-id="00a2a-134">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-134">String</span></span>|<span data-ttu-id="00a2a-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="00a2a-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="00a2a-136">eventDateTime</span></span>|<span data-ttu-id="00a2a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a2a-137">DateTimeOffset</span></span>|<span data-ttu-id="00a2a-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="00a2a-138">Time when the event occurred .</span></span> <span data-ttu-id="00a2a-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="00a2a-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="00a2a-140">correlationId</span></span>|<span data-ttu-id="00a2a-141">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-141">String</span></span>|<span data-ttu-id="00a2a-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="00a2a-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="00a2a-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="00a2a-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="00a2a-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="00a2a-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="00a2a-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="00a2a-146">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="00a2a-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="00a2a-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="00a2a-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-148">名</span><span class="sxs-lookup"><span data-stu-id="00a2a-148">eventName</span></span>|<span data-ttu-id="00a2a-149">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-149">String</span></span>|<span data-ttu-id="00a2a-150">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="00a2a-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="00a2a-151">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="00a2a-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="00a2a-152">additionalInformation</span></span>|<span data-ttu-id="00a2a-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00a2a-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="00a2a-154">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="00a2a-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="00a2a-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="00a2a-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="00a2a-156">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-156">String</span></span>|<span data-ttu-id="00a2a-157">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="00a2a-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="00a2a-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="00a2a-158">operatingSystem</span></span>|<span data-ttu-id="00a2a-159">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-159">String</span></span>|<span data-ttu-id="00a2a-160">操作系统。</span><span class="sxs-lookup"><span data-stu-id="00a2a-160">Operating System.</span></span>|
|<span data-ttu-id="00a2a-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="00a2a-161">osVersion</span></span>|<span data-ttu-id="00a2a-162">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-162">String</span></span>|<span data-ttu-id="00a2a-163">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="00a2a-163">OS Version.</span></span>|
|<span data-ttu-id="00a2a-164">userId</span><span class="sxs-lookup"><span data-stu-id="00a2a-164">userId</span></span>|<span data-ttu-id="00a2a-165">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-165">String</span></span>|<span data-ttu-id="00a2a-166">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="00a2a-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="00a2a-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="00a2a-167">deviceId</span></span>|<span data-ttu-id="00a2a-168">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-168">String</span></span>|<span data-ttu-id="00a2a-169">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="00a2a-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="00a2a-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="00a2a-170">enrollmentType</span></span>|[<span data-ttu-id="00a2a-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="00a2a-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="00a2a-172">注册类型。</span><span class="sxs-lookup"><span data-stu-id="00a2a-172">Type of the enrollment.</span></span> <span data-ttu-id="00a2a-173">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="00a2a-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="00a2a-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="00a2a-174">failureCategory</span></span>|[<span data-ttu-id="00a2a-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="00a2a-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="00a2a-176">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="00a2a-176">Highlevel failure category.</span></span> <span data-ttu-id="00a2a-177">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="00a2a-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="00a2a-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="00a2a-178">failureReason</span></span>|<span data-ttu-id="00a2a-179">String</span><span class="sxs-lookup"><span data-stu-id="00a2a-179">String</span></span>|<span data-ttu-id="00a2a-180">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="00a2a-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="00a2a-181">响应</span><span class="sxs-lookup"><span data-stu-id="00a2a-181">Response</span></span>
<span data-ttu-id="00a2a-182">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00a2a-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00a2a-183">示例</span><span class="sxs-lookup"><span data-stu-id="00a2a-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="00a2a-184">请求</span><span class="sxs-lookup"><span data-stu-id="00a2a-184">Request</span></span>
<span data-ttu-id="00a2a-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00a2a-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00a2a-186">响应</span><span class="sxs-lookup"><span data-stu-id="00a2a-186">Response</span></span>
<span data-ttu-id="00a2a-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00a2a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





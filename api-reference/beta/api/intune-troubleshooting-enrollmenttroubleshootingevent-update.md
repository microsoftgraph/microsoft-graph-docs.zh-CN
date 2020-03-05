---
title: 更新 enrollmentTroubleshootingEvent
description: 更新 enrollmentTroubleshootingEvent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1fa294b068f1eb98d55e395091ca0b0a145f96f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457634"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="8e570-103">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8e570-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="8e570-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8e570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e570-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e570-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e570-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e570-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e570-107">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e570-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e570-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e570-108">Prerequisites</span></span>
<span data-ttu-id="8e570-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e570-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e570-111">Permission type</span></span>|<span data-ttu-id="8e570-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e570-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e570-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e570-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e570-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e570-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e570-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e570-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e570-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e570-116">Not supported.</span></span>|
|<span data-ttu-id="8e570-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e570-117">Application</span></span>|<span data-ttu-id="8e570-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e570-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e570-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e570-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="8e570-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e570-120">Request headers</span></span>
|<span data-ttu-id="8e570-121">标头</span><span class="sxs-lookup"><span data-stu-id="8e570-121">Header</span></span>|<span data-ttu-id="8e570-122">值</span><span class="sxs-lookup"><span data-stu-id="8e570-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e570-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e570-123">Authorization</span></span>|<span data-ttu-id="8e570-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e570-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e570-125">接受</span><span class="sxs-lookup"><span data-stu-id="8e570-125">Accept</span></span>|<span data-ttu-id="8e570-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e570-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e570-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e570-127">Request body</span></span>
<span data-ttu-id="8e570-128">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e570-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="8e570-129">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8e570-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="8e570-130">属性</span><span class="sxs-lookup"><span data-stu-id="8e570-130">Property</span></span>|<span data-ttu-id="8e570-131">类型</span><span class="sxs-lookup"><span data-stu-id="8e570-131">Type</span></span>|<span data-ttu-id="8e570-132">说明</span><span class="sxs-lookup"><span data-stu-id="8e570-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e570-133">id</span><span class="sxs-lookup"><span data-stu-id="8e570-133">id</span></span>|<span data-ttu-id="8e570-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8e570-134">String</span></span>|<span data-ttu-id="8e570-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e570-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8e570-136">eventDateTime</span></span>|<span data-ttu-id="8e570-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e570-137">DateTimeOffset</span></span>|<span data-ttu-id="8e570-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8e570-138">Time when the event occurred .</span></span> <span data-ttu-id="8e570-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e570-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="8e570-140">correlationId</span></span>|<span data-ttu-id="8e570-141">String</span><span class="sxs-lookup"><span data-stu-id="8e570-141">String</span></span>|<span data-ttu-id="8e570-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="8e570-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8e570-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e570-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8e570-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="8e570-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8e570-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="8e570-146">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="8e570-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="8e570-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e570-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-148">名</span><span class="sxs-lookup"><span data-stu-id="8e570-148">eventName</span></span>|<span data-ttu-id="8e570-149">String</span><span class="sxs-lookup"><span data-stu-id="8e570-149">String</span></span>|<span data-ttu-id="8e570-150">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="8e570-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="8e570-151">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="8e570-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="8e570-152">additionalInformation</span></span>|<span data-ttu-id="8e570-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e570-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8e570-154">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="8e570-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e570-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e570-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="8e570-156">String</span><span class="sxs-lookup"><span data-stu-id="8e570-156">String</span></span>|<span data-ttu-id="8e570-157">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="8e570-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8e570-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e570-158">operatingSystem</span></span>|<span data-ttu-id="8e570-159">String</span><span class="sxs-lookup"><span data-stu-id="8e570-159">String</span></span>|<span data-ttu-id="8e570-160">操作系统。</span><span class="sxs-lookup"><span data-stu-id="8e570-160">Operating System.</span></span>|
|<span data-ttu-id="8e570-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="8e570-161">osVersion</span></span>|<span data-ttu-id="8e570-162">String</span><span class="sxs-lookup"><span data-stu-id="8e570-162">String</span></span>|<span data-ttu-id="8e570-163">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8e570-163">OS Version.</span></span>|
|<span data-ttu-id="8e570-164">userId</span><span class="sxs-lookup"><span data-stu-id="8e570-164">userId</span></span>|<span data-ttu-id="8e570-165">String</span><span class="sxs-lookup"><span data-stu-id="8e570-165">String</span></span>|<span data-ttu-id="8e570-166">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="8e570-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8e570-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="8e570-167">deviceId</span></span>|<span data-ttu-id="8e570-168">String</span><span class="sxs-lookup"><span data-stu-id="8e570-168">String</span></span>|<span data-ttu-id="8e570-169">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="8e570-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8e570-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e570-170">enrollmentType</span></span>|[<span data-ttu-id="8e570-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e570-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8e570-172">注册类型。</span><span class="sxs-lookup"><span data-stu-id="8e570-172">Type of the enrollment.</span></span> <span data-ttu-id="8e570-173">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="8e570-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="8e570-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8e570-174">failureCategory</span></span>|[<span data-ttu-id="8e570-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="8e570-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="8e570-176">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="8e570-176">Highlevel failure category.</span></span> <span data-ttu-id="8e570-177">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="8e570-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="8e570-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="8e570-178">failureReason</span></span>|<span data-ttu-id="8e570-179">String</span><span class="sxs-lookup"><span data-stu-id="8e570-179">String</span></span>|<span data-ttu-id="8e570-180">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="8e570-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8e570-181">响应</span><span class="sxs-lookup"><span data-stu-id="8e570-181">Response</span></span>
<span data-ttu-id="8e570-182">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e570-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e570-183">示例</span><span class="sxs-lookup"><span data-stu-id="8e570-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e570-184">请求</span><span class="sxs-lookup"><span data-stu-id="8e570-184">Request</span></span>
<span data-ttu-id="8e570-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e570-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e570-186">响应</span><span class="sxs-lookup"><span data-stu-id="8e570-186">Response</span></span>
<span data-ttu-id="8e570-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e570-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






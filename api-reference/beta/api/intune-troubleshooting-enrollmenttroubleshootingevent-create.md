---
title: 创建 enrollmentTroubleshootingEvent
description: 创建新的 enrollmentTroubleshootingEvent 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df7c2d85458811684c7d8593c5f9f85c102bbd96
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990811"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="f21eb-103">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f21eb-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="f21eb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f21eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f21eb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f21eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f21eb-106">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f21eb-106">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f21eb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f21eb-107">Prerequisites</span></span>
<span data-ttu-id="f21eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f21eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f21eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f21eb-110">Permission type</span></span>|<span data-ttu-id="f21eb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f21eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f21eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f21eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f21eb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21eb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f21eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f21eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f21eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f21eb-115">Not supported.</span></span>|
|<span data-ttu-id="f21eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f21eb-116">Application</span></span>|<span data-ttu-id="f21eb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f21eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f21eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f21eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f21eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f21eb-119">Request headers</span></span>
|<span data-ttu-id="f21eb-120">标头</span><span class="sxs-lookup"><span data-stu-id="f21eb-120">Header</span></span>|<span data-ttu-id="f21eb-121">值</span><span class="sxs-lookup"><span data-stu-id="f21eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f21eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f21eb-122">Authorization</span></span>|<span data-ttu-id="f21eb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f21eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f21eb-124">接受</span><span class="sxs-lookup"><span data-stu-id="f21eb-124">Accept</span></span>|<span data-ttu-id="f21eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f21eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f21eb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f21eb-126">Request body</span></span>
<span data-ttu-id="f21eb-127">在请求正文中，提供 enrollmentTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f21eb-127">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="f21eb-128">下表显示创建 enrollmentTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f21eb-128">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="f21eb-129">属性</span><span class="sxs-lookup"><span data-stu-id="f21eb-129">Property</span></span>|<span data-ttu-id="f21eb-130">类型</span><span class="sxs-lookup"><span data-stu-id="f21eb-130">Type</span></span>|<span data-ttu-id="f21eb-131">说明</span><span class="sxs-lookup"><span data-stu-id="f21eb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21eb-132">id</span><span class="sxs-lookup"><span data-stu-id="f21eb-132">id</span></span>|<span data-ttu-id="f21eb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f21eb-133">String</span></span>|<span data-ttu-id="f21eb-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f21eb-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f21eb-135">eventDateTime</span></span>|<span data-ttu-id="f21eb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21eb-136">DateTimeOffset</span></span>|<span data-ttu-id="f21eb-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f21eb-137">Time when the event occurred .</span></span> <span data-ttu-id="f21eb-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f21eb-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="f21eb-139">correlationId</span></span>|<span data-ttu-id="f21eb-140">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-140">String</span></span>|<span data-ttu-id="f21eb-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="f21eb-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="f21eb-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f21eb-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f21eb-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f21eb-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f21eb-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f21eb-145">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="f21eb-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="f21eb-146">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f21eb-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-147">名</span><span class="sxs-lookup"><span data-stu-id="f21eb-147">eventName</span></span>|<span data-ttu-id="f21eb-148">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-148">String</span></span>|<span data-ttu-id="f21eb-149">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="f21eb-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="f21eb-150">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="f21eb-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="f21eb-151">additionalInformation</span></span>|<span data-ttu-id="f21eb-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f21eb-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f21eb-153">一组字符串键和字符串值对, 提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="f21eb-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f21eb-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f21eb-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="f21eb-155">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-155">String</span></span>|<span data-ttu-id="f21eb-156">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f21eb-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f21eb-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f21eb-157">operatingSystem</span></span>|<span data-ttu-id="f21eb-158">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-158">String</span></span>|<span data-ttu-id="f21eb-159">操作系统。</span><span class="sxs-lookup"><span data-stu-id="f21eb-159">Operating System.</span></span>|
|<span data-ttu-id="f21eb-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="f21eb-160">osVersion</span></span>|<span data-ttu-id="f21eb-161">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-161">String</span></span>|<span data-ttu-id="f21eb-162">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f21eb-162">OS Version.</span></span>|
|<span data-ttu-id="f21eb-163">userId</span><span class="sxs-lookup"><span data-stu-id="f21eb-163">userId</span></span>|<span data-ttu-id="f21eb-164">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-164">String</span></span>|<span data-ttu-id="f21eb-165">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="f21eb-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f21eb-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="f21eb-166">deviceId</span></span>|<span data-ttu-id="f21eb-167">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-167">String</span></span>|<span data-ttu-id="f21eb-168">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f21eb-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="f21eb-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="f21eb-169">enrollmentType</span></span>|[<span data-ttu-id="f21eb-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f21eb-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f21eb-171">注册类型。</span><span class="sxs-lookup"><span data-stu-id="f21eb-171">Type of the enrollment.</span></span> <span data-ttu-id="f21eb-172">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="f21eb-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f21eb-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="f21eb-173">failureCategory</span></span>|[<span data-ttu-id="f21eb-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="f21eb-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="f21eb-175">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="f21eb-175">Highlevel failure category.</span></span> <span data-ttu-id="f21eb-176">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="f21eb-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="f21eb-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="f21eb-177">failureReason</span></span>|<span data-ttu-id="f21eb-178">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-178">String</span></span>|<span data-ttu-id="f21eb-179">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="f21eb-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="f21eb-180">响应</span><span class="sxs-lookup"><span data-stu-id="f21eb-180">Response</span></span>
<span data-ttu-id="f21eb-181">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f21eb-181">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f21eb-182">示例</span><span class="sxs-lookup"><span data-stu-id="f21eb-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="f21eb-183">请求</span><span class="sxs-lookup"><span data-stu-id="f21eb-183">Request</span></span>
<span data-ttu-id="f21eb-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f21eb-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="f21eb-185">响应</span><span class="sxs-lookup"><span data-stu-id="f21eb-185">Response</span></span>
<span data-ttu-id="f21eb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f21eb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






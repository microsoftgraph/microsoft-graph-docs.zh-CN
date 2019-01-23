---
title: 创建 enrollmentTroubleshootingEvent
description: 创建新的 enrollmentTroubleshootingEvent 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a9eefb12628bf3d95c94b913ec8ae66a90108d08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418972"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="f90af-103">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f90af-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="f90af-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f90af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f90af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f90af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f90af-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f90af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f90af-107">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f90af-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f90af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f90af-108">Prerequisites</span></span>
<span data-ttu-id="f90af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f90af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f90af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f90af-111">Permission type</span></span>|<span data-ttu-id="f90af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f90af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f90af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f90af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f90af-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f90af-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f90af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f90af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f90af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f90af-116">Not supported.</span></span>|
|<span data-ttu-id="f90af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f90af-117">Application</span></span>|<span data-ttu-id="f90af-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f90af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f90af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f90af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f90af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f90af-120">Request headers</span></span>
|<span data-ttu-id="f90af-121">标头</span><span class="sxs-lookup"><span data-stu-id="f90af-121">Header</span></span>|<span data-ttu-id="f90af-122">值</span><span class="sxs-lookup"><span data-stu-id="f90af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f90af-123">授权</span><span class="sxs-lookup"><span data-stu-id="f90af-123">Authorization</span></span>|<span data-ttu-id="f90af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f90af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f90af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f90af-125">Accept</span></span>|<span data-ttu-id="f90af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f90af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f90af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f90af-127">Request body</span></span>
<span data-ttu-id="f90af-128">在请求正文中，提供 enrollmentTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f90af-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="f90af-129">下表显示创建 enrollmentTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f90af-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="f90af-130">属性</span><span class="sxs-lookup"><span data-stu-id="f90af-130">Property</span></span>|<span data-ttu-id="f90af-131">类型</span><span class="sxs-lookup"><span data-stu-id="f90af-131">Type</span></span>|<span data-ttu-id="f90af-132">说明</span><span class="sxs-lookup"><span data-stu-id="f90af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f90af-133">id</span><span class="sxs-lookup"><span data-stu-id="f90af-133">id</span></span>|<span data-ttu-id="f90af-134">String</span><span class="sxs-lookup"><span data-stu-id="f90af-134">String</span></span>|<span data-ttu-id="f90af-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f90af-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f90af-136">eventDateTime</span></span>|<span data-ttu-id="f90af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90af-137">DateTimeOffset</span></span>|<span data-ttu-id="f90af-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f90af-138">Time when the event occurred .</span></span> <span data-ttu-id="f90af-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f90af-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="f90af-140">correlationId</span></span>|<span data-ttu-id="f90af-141">String</span><span class="sxs-lookup"><span data-stu-id="f90af-141">String</span></span>|<span data-ttu-id="f90af-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="f90af-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="f90af-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f90af-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f90af-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f90af-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f90af-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f90af-146">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="f90af-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="f90af-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f90af-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-148">事件名称</span><span class="sxs-lookup"><span data-stu-id="f90af-148">eventName</span></span>|<span data-ttu-id="f90af-149">String</span><span class="sxs-lookup"><span data-stu-id="f90af-149">String</span></span>|<span data-ttu-id="f90af-150">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="f90af-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="f90af-151">它是一个可选字段继承从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f90af-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="f90af-152">additionalInformation</span></span>|<span data-ttu-id="f90af-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f90af-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f90af-154">一组字符串键和字符串值对提供了有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)疑难解答事件继承其他信息</span><span class="sxs-lookup"><span data-stu-id="f90af-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f90af-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f90af-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="f90af-156">String</span><span class="sxs-lookup"><span data-stu-id="f90af-156">String</span></span>|<span data-ttu-id="f90af-157">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f90af-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f90af-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f90af-158">operatingSystem</span></span>|<span data-ttu-id="f90af-159">String</span><span class="sxs-lookup"><span data-stu-id="f90af-159">String</span></span>|<span data-ttu-id="f90af-160">操作系统。</span><span class="sxs-lookup"><span data-stu-id="f90af-160">Operating System.</span></span>|
|<span data-ttu-id="f90af-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="f90af-161">osVersion</span></span>|<span data-ttu-id="f90af-162">String</span><span class="sxs-lookup"><span data-stu-id="f90af-162">String</span></span>|<span data-ttu-id="f90af-163">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f90af-163">OS Version.</span></span>|
|<span data-ttu-id="f90af-164">userId</span><span class="sxs-lookup"><span data-stu-id="f90af-164">userId</span></span>|<span data-ttu-id="f90af-165">String</span><span class="sxs-lookup"><span data-stu-id="f90af-165">String</span></span>|<span data-ttu-id="f90af-166">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="f90af-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f90af-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="f90af-167">deviceId</span></span>|<span data-ttu-id="f90af-168">String</span><span class="sxs-lookup"><span data-stu-id="f90af-168">String</span></span>|<span data-ttu-id="f90af-169">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f90af-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="f90af-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="f90af-170">enrollmentType</span></span>|[<span data-ttu-id="f90af-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f90af-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f90af-172">注册类型。</span><span class="sxs-lookup"><span data-stu-id="f90af-172">Type of the enrollment.</span></span> <span data-ttu-id="f90af-173">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="f90af-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f90af-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="f90af-174">failureCategory</span></span>|[<span data-ttu-id="f90af-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="f90af-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="f90af-176">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="f90af-176">Highlevel failure category.</span></span> <span data-ttu-id="f90af-177">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="f90af-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="f90af-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="f90af-178">failureReason</span></span>|<span data-ttu-id="f90af-179">String</span><span class="sxs-lookup"><span data-stu-id="f90af-179">String</span></span>|<span data-ttu-id="f90af-180">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="f90af-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="f90af-181">响应</span><span class="sxs-lookup"><span data-stu-id="f90af-181">Response</span></span>
<span data-ttu-id="f90af-182">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f90af-182">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f90af-183">示例</span><span class="sxs-lookup"><span data-stu-id="f90af-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="f90af-184">请求</span><span class="sxs-lookup"><span data-stu-id="f90af-184">Request</span></span>
<span data-ttu-id="f90af-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f90af-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f90af-186">响应</span><span class="sxs-lookup"><span data-stu-id="f90af-186">Response</span></span>
<span data-ttu-id="f90af-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f90af-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





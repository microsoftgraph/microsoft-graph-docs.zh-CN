---
title: 更新 enrollmentTroubleshootingEvent
description: 更新 enrollmentTroubleshootingEvent 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 981228381902bb2b0dfa1296285de6cfa271286c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511836"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="41165-103">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="41165-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="41165-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41165-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41165-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41165-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41165-106">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41165-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41165-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41165-107">Prerequisites</span></span>
<span data-ttu-id="41165-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41165-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41165-110">Permission type</span></span>|<span data-ttu-id="41165-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41165-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41165-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41165-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41165-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41165-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="41165-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41165-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41165-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41165-115">Not supported.</span></span>|
|<span data-ttu-id="41165-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41165-116">Application</span></span>|<span data-ttu-id="41165-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41165-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41165-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41165-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="41165-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41165-119">Request headers</span></span>
|<span data-ttu-id="41165-120">标头</span><span class="sxs-lookup"><span data-stu-id="41165-120">Header</span></span>|<span data-ttu-id="41165-121">值</span><span class="sxs-lookup"><span data-stu-id="41165-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41165-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41165-122">Authorization</span></span>|<span data-ttu-id="41165-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41165-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41165-124">接受</span><span class="sxs-lookup"><span data-stu-id="41165-124">Accept</span></span>|<span data-ttu-id="41165-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41165-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41165-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41165-126">Request body</span></span>
<span data-ttu-id="41165-127">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41165-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="41165-128">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41165-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="41165-129">属性</span><span class="sxs-lookup"><span data-stu-id="41165-129">Property</span></span>|<span data-ttu-id="41165-130">类型</span><span class="sxs-lookup"><span data-stu-id="41165-130">Type</span></span>|<span data-ttu-id="41165-131">说明</span><span class="sxs-lookup"><span data-stu-id="41165-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41165-132">id</span><span class="sxs-lookup"><span data-stu-id="41165-132">id</span></span>|<span data-ttu-id="41165-133">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-133">String</span></span>|<span data-ttu-id="41165-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="41165-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="41165-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="41165-135">eventDateTime</span></span>|<span data-ttu-id="41165-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41165-136">DateTimeOffset</span></span>|<span data-ttu-id="41165-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="41165-137">Time when the event occurred .</span></span> <span data-ttu-id="41165-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="41165-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="41165-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="41165-139">correlationId</span></span>|<span data-ttu-id="41165-140">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-140">String</span></span>|<span data-ttu-id="41165-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="41165-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="41165-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="41165-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="41165-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="41165-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="41165-144">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-144">String</span></span>|<span data-ttu-id="41165-145">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="41165-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="41165-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="41165-146">operatingSystem</span></span>|<span data-ttu-id="41165-147">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-147">String</span></span>|<span data-ttu-id="41165-148">操作系统。</span><span class="sxs-lookup"><span data-stu-id="41165-148">Operating System.</span></span>|
|<span data-ttu-id="41165-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="41165-149">osVersion</span></span>|<span data-ttu-id="41165-150">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-150">String</span></span>|<span data-ttu-id="41165-151">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="41165-151">OS Version.</span></span>|
|<span data-ttu-id="41165-152">userId</span><span class="sxs-lookup"><span data-stu-id="41165-152">userId</span></span>|<span data-ttu-id="41165-153">String</span><span class="sxs-lookup"><span data-stu-id="41165-153">String</span></span>|<span data-ttu-id="41165-154">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="41165-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="41165-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="41165-155">deviceId</span></span>|<span data-ttu-id="41165-156">字符串</span><span class="sxs-lookup"><span data-stu-id="41165-156">String</span></span>|<span data-ttu-id="41165-157">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="41165-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="41165-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="41165-158">enrollmentType</span></span>|[<span data-ttu-id="41165-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="41165-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="41165-160">注册类型。</span><span class="sxs-lookup"><span data-stu-id="41165-160">Type of the enrollment.</span></span> <span data-ttu-id="41165-161">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="41165-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="41165-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="41165-162">failureCategory</span></span>|[<span data-ttu-id="41165-163">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="41165-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="41165-164">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="41165-164">Highlevel failure category.</span></span> <span data-ttu-id="41165-165">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="41165-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="41165-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="41165-166">failureReason</span></span>|<span data-ttu-id="41165-167">String</span><span class="sxs-lookup"><span data-stu-id="41165-167">String</span></span>|<span data-ttu-id="41165-168">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="41165-168">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="41165-169">响应</span><span class="sxs-lookup"><span data-stu-id="41165-169">Response</span></span>
<span data-ttu-id="41165-170">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41165-170">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41165-171">示例</span><span class="sxs-lookup"><span data-stu-id="41165-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="41165-172">请求</span><span class="sxs-lookup"><span data-stu-id="41165-172">Request</span></span>
<span data-ttu-id="41165-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41165-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
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

### <a name="response"></a><span data-ttu-id="41165-174">响应</span><span class="sxs-lookup"><span data-stu-id="41165-174">Response</span></span>
<span data-ttu-id="41165-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41165-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
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





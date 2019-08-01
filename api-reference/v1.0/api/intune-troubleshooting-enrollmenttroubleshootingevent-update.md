---
title: 更新 enrollmentTroubleshootingEvent
description: 更新 enrollmentTroubleshootingEvent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e17167d2965102618d0033210a69b39db16686a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025636"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="67fb3-103">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="67fb3-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="67fb3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67fb3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fb3-105">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="67fb3-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67fb3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="67fb3-106">Prerequisites</span></span>
<span data-ttu-id="67fb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67fb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67fb3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67fb3-109">Permission type</span></span>|<span data-ttu-id="67fb3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67fb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67fb3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67fb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67fb3-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fb3-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="67fb3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67fb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67fb3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="67fb3-114">Not supported.</span></span>|
|<span data-ttu-id="67fb3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67fb3-115">Application</span></span>|<span data-ttu-id="67fb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67fb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67fb3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67fb3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="67fb3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="67fb3-118">Request headers</span></span>
|<span data-ttu-id="67fb3-119">标头</span><span class="sxs-lookup"><span data-stu-id="67fb3-119">Header</span></span>|<span data-ttu-id="67fb3-120">值</span><span class="sxs-lookup"><span data-stu-id="67fb3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67fb3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67fb3-121">Authorization</span></span>|<span data-ttu-id="67fb3-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67fb3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67fb3-123">接受</span><span class="sxs-lookup"><span data-stu-id="67fb3-123">Accept</span></span>|<span data-ttu-id="67fb3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67fb3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67fb3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="67fb3-125">Request body</span></span>
<span data-ttu-id="67fb3-126">在请求正文中，提供 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67fb3-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="67fb3-127">下表显示创建 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67fb3-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="67fb3-128">属性</span><span class="sxs-lookup"><span data-stu-id="67fb3-128">Property</span></span>|<span data-ttu-id="67fb3-129">类型</span><span class="sxs-lookup"><span data-stu-id="67fb3-129">Type</span></span>|<span data-ttu-id="67fb3-130">说明</span><span class="sxs-lookup"><span data-stu-id="67fb3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fb3-131">id</span><span class="sxs-lookup"><span data-stu-id="67fb3-131">id</span></span>|<span data-ttu-id="67fb3-132">字符串</span><span class="sxs-lookup"><span data-stu-id="67fb3-132">String</span></span>|<span data-ttu-id="67fb3-133">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="67fb3-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="67fb3-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="67fb3-134">eventDateTime</span></span>|<span data-ttu-id="67fb3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fb3-135">DateTimeOffset</span></span>|<span data-ttu-id="67fb3-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="67fb3-136">Time when the event occurred .</span></span> <span data-ttu-id="67fb3-137">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="67fb3-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="67fb3-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="67fb3-138">correlationId</span></span>|<span data-ttu-id="67fb3-139">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-139">String</span></span>|<span data-ttu-id="67fb3-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="67fb3-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="67fb3-141">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="67fb3-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="67fb3-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="67fb3-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="67fb3-143">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-143">String</span></span>|<span data-ttu-id="67fb3-144">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="67fb3-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="67fb3-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="67fb3-145">operatingSystem</span></span>|<span data-ttu-id="67fb3-146">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-146">String</span></span>|<span data-ttu-id="67fb3-147">操作系统。</span><span class="sxs-lookup"><span data-stu-id="67fb3-147">Operating System.</span></span>|
|<span data-ttu-id="67fb3-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="67fb3-148">osVersion</span></span>|<span data-ttu-id="67fb3-149">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-149">String</span></span>|<span data-ttu-id="67fb3-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="67fb3-150">OS Version.</span></span>|
|<span data-ttu-id="67fb3-151">userId</span><span class="sxs-lookup"><span data-stu-id="67fb3-151">userId</span></span>|<span data-ttu-id="67fb3-152">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-152">String</span></span>|<span data-ttu-id="67fb3-153">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="67fb3-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="67fb3-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="67fb3-154">deviceId</span></span>|<span data-ttu-id="67fb3-155">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-155">String</span></span>|<span data-ttu-id="67fb3-156">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="67fb3-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="67fb3-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="67fb3-157">enrollmentType</span></span>|[<span data-ttu-id="67fb3-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="67fb3-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="67fb3-159">注册类型。</span><span class="sxs-lookup"><span data-stu-id="67fb3-159">Type of the enrollment.</span></span> <span data-ttu-id="67fb3-160">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="67fb3-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="67fb3-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="67fb3-161">failureCategory</span></span>|[<span data-ttu-id="67fb3-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="67fb3-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="67fb3-163">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="67fb3-163">Highlevel failure category.</span></span> <span data-ttu-id="67fb3-164">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="67fb3-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="67fb3-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="67fb3-165">failureReason</span></span>|<span data-ttu-id="67fb3-166">String</span><span class="sxs-lookup"><span data-stu-id="67fb3-166">String</span></span>|<span data-ttu-id="67fb3-167">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="67fb3-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="67fb3-168">响应</span><span class="sxs-lookup"><span data-stu-id="67fb3-168">Response</span></span>
<span data-ttu-id="67fb3-169">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67fb3-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67fb3-170">示例</span><span class="sxs-lookup"><span data-stu-id="67fb3-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="67fb3-171">请求</span><span class="sxs-lookup"><span data-stu-id="67fb3-171">Request</span></span>
<span data-ttu-id="67fb3-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67fb3-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67fb3-173">响应</span><span class="sxs-lookup"><span data-stu-id="67fb3-173">Response</span></span>
<span data-ttu-id="67fb3-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67fb3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




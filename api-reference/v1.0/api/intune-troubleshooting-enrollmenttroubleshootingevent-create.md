---
title: 创建 enrollmentTroubleshootingEvent
description: 创建新的 enrollmentTroubleshootingEvent 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64894d39d38359331815818c6342d46dae35d09a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361026"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="f2c5b-103">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f2c5b-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="f2c5b-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2c5b-105">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2c5b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2c5b-106">Prerequisites</span></span>
<span data-ttu-id="f2c5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c5b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2c5b-109">Permission type</span></span>|<span data-ttu-id="f2c5b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2c5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c5b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c5b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2c5b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c5b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2c5b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c5b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c5b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-114">Not supported.</span></span>|
|<span data-ttu-id="f2c5b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2c5b-115">Application</span></span>|<span data-ttu-id="f2c5b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2c5b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2c5b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f2c5b-118">请求头</span><span class="sxs-lookup"><span data-stu-id="f2c5b-118">Request headers</span></span>
|<span data-ttu-id="f2c5b-119">标头</span><span class="sxs-lookup"><span data-stu-id="f2c5b-119">Header</span></span>|<span data-ttu-id="f2c5b-120">值</span><span class="sxs-lookup"><span data-stu-id="f2c5b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2c5b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c5b-121">Authorization</span></span>|<span data-ttu-id="f2c5b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2c5b-123">接受</span><span class="sxs-lookup"><span data-stu-id="f2c5b-123">Accept</span></span>|<span data-ttu-id="f2c5b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2c5b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c5b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2c5b-125">Request body</span></span>
<span data-ttu-id="f2c5b-126">在请求正文中，提供 enrollmentTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="f2c5b-127">下表显示创建 enrollmentTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="f2c5b-128">属性</span><span class="sxs-lookup"><span data-stu-id="f2c5b-128">Property</span></span>|<span data-ttu-id="f2c5b-129">类型</span><span class="sxs-lookup"><span data-stu-id="f2c5b-129">Type</span></span>|<span data-ttu-id="f2c5b-130">说明</span><span class="sxs-lookup"><span data-stu-id="f2c5b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2c5b-131">id</span><span class="sxs-lookup"><span data-stu-id="f2c5b-131">id</span></span>|<span data-ttu-id="f2c5b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="f2c5b-132">String</span></span>|<span data-ttu-id="f2c5b-133">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f2c5b-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f2c5b-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f2c5b-134">eventDateTime</span></span>|<span data-ttu-id="f2c5b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2c5b-135">DateTimeOffset</span></span>|<span data-ttu-id="f2c5b-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-136">Time when the event occurred .</span></span> <span data-ttu-id="f2c5b-137">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f2c5b-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f2c5b-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="f2c5b-138">correlationId</span></span>|<span data-ttu-id="f2c5b-139">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-139">String</span></span>|<span data-ttu-id="f2c5b-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="f2c5b-141">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f2c5b-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f2c5b-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2c5b-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="f2c5b-143">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-143">String</span></span>|<span data-ttu-id="f2c5b-144">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f2c5b-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2c5b-145">operatingSystem</span></span>|<span data-ttu-id="f2c5b-146">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-146">String</span></span>|<span data-ttu-id="f2c5b-147">操作系统。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-147">Operating System.</span></span>|
|<span data-ttu-id="f2c5b-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="f2c5b-148">osVersion</span></span>|<span data-ttu-id="f2c5b-149">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-149">String</span></span>|<span data-ttu-id="f2c5b-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-150">OS Version.</span></span>|
|<span data-ttu-id="f2c5b-151">userId</span><span class="sxs-lookup"><span data-stu-id="f2c5b-151">userId</span></span>|<span data-ttu-id="f2c5b-152">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-152">String</span></span>|<span data-ttu-id="f2c5b-153">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f2c5b-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="f2c5b-154">deviceId</span></span>|<span data-ttu-id="f2c5b-155">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-155">String</span></span>|<span data-ttu-id="f2c5b-156">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="f2c5b-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="f2c5b-157">enrollmentType</span></span>|[<span data-ttu-id="f2c5b-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f2c5b-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f2c5b-159">注册类型。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-159">Type of the enrollment.</span></span> <span data-ttu-id="f2c5b-160">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f2c5b-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="f2c5b-161">failureCategory</span></span>|[<span data-ttu-id="f2c5b-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="f2c5b-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="f2c5b-163">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-163">Highlevel failure category.</span></span> <span data-ttu-id="f2c5b-164">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="f2c5b-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="f2c5b-165">failureReason</span></span>|<span data-ttu-id="f2c5b-166">String</span><span class="sxs-lookup"><span data-stu-id="f2c5b-166">String</span></span>|<span data-ttu-id="f2c5b-167">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="f2c5b-168">响应</span><span class="sxs-lookup"><span data-stu-id="f2c5b-168">Response</span></span>
<span data-ttu-id="f2c5b-169">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2c5b-170">示例</span><span class="sxs-lookup"><span data-stu-id="f2c5b-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2c5b-171">请求</span><span class="sxs-lookup"><span data-stu-id="f2c5b-171">Request</span></span>
<span data-ttu-id="f2c5b-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="f2c5b-173">响应</span><span class="sxs-lookup"><span data-stu-id="f2c5b-173">Response</span></span>
<span data-ttu-id="f2c5b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2c5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





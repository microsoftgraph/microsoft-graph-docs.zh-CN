---
title: 创建 enrollmentTroubleshootingEvent
description: 创建新的 enrollmentTroubleshootingEvent 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94e3f1f98a8400d7794863e7b3852d50be97b712
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872686"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="8fb9e-103">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8fb9e-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="8fb9e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fb9e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fb9e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fb9e-107">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fb9e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8fb9e-108">Prerequisites</span></span>
<span data-ttu-id="8fb9e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8fb9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb9e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fb9e-111">Permission type</span></span>|<span data-ttu-id="8fb9e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8fb9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fb9e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fb9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fb9e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb9e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8fb9e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fb9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fb9e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-116">Not supported.</span></span>|
|<span data-ttu-id="8fb9e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fb9e-117">Application</span></span>|<span data-ttu-id="8fb9e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fb9e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fb9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8fb9e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fb9e-120">Request headers</span></span>
|<span data-ttu-id="8fb9e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8fb9e-121">Header</span></span>|<span data-ttu-id="8fb9e-122">值</span><span class="sxs-lookup"><span data-stu-id="8fb9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fb9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fb9e-123">Authorization</span></span>|<span data-ttu-id="8fb9e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fb9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8fb9e-125">Accept</span></span>|<span data-ttu-id="8fb9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fb9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fb9e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fb9e-127">Request body</span></span>
<span data-ttu-id="8fb9e-128">在请求正文中，提供 enrollmentTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="8fb9e-129">下表显示创建 enrollmentTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="8fb9e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8fb9e-130">Property</span></span>|<span data-ttu-id="8fb9e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8fb9e-131">Type</span></span>|<span data-ttu-id="8fb9e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8fb9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb9e-133">id</span><span class="sxs-lookup"><span data-stu-id="8fb9e-133">id</span></span>|<span data-ttu-id="8fb9e-134">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-134">String</span></span>|<span data-ttu-id="8fb9e-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8fb9e-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8fb9e-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb9e-136">eventDateTime</span></span>|<span data-ttu-id="8fb9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb9e-137">DateTimeOffset</span></span>|<span data-ttu-id="8fb9e-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-138">Time when the event occurred .</span></span> <span data-ttu-id="8fb9e-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8fb9e-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8fb9e-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="8fb9e-140">correlationId</span></span>|<span data-ttu-id="8fb9e-141">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-141">String</span></span>|<span data-ttu-id="8fb9e-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8fb9e-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8fb9e-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8fb9e-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8fb9e-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="8fb9e-145">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-145">String</span></span>|<span data-ttu-id="8fb9e-146">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8fb9e-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8fb9e-147">operatingSystem</span></span>|<span data-ttu-id="8fb9e-148">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-148">String</span></span>|<span data-ttu-id="8fb9e-149">操作系统。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-149">Operating System.</span></span>|
|<span data-ttu-id="8fb9e-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="8fb9e-150">osVersion</span></span>|<span data-ttu-id="8fb9e-151">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-151">String</span></span>|<span data-ttu-id="8fb9e-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-152">OS Version.</span></span>|
|<span data-ttu-id="8fb9e-153">userId</span><span class="sxs-lookup"><span data-stu-id="8fb9e-153">userId</span></span>|<span data-ttu-id="8fb9e-154">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-154">String</span></span>|<span data-ttu-id="8fb9e-155">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8fb9e-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="8fb9e-156">deviceId</span></span>|<span data-ttu-id="8fb9e-157">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-157">String</span></span>|<span data-ttu-id="8fb9e-158">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8fb9e-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8fb9e-159">enrollmentType</span></span>|[<span data-ttu-id="8fb9e-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8fb9e-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8fb9e-161">注册类型。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-161">Type of the enrollment.</span></span> <span data-ttu-id="8fb9e-162">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="8fb9e-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8fb9e-163">failureCategory</span></span>|[<span data-ttu-id="8fb9e-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="8fb9e-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="8fb9e-165">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-165">Highlevel failure category.</span></span> <span data-ttu-id="8fb9e-166">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="8fb9e-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="8fb9e-167">failureReason</span></span>|<span data-ttu-id="8fb9e-168">String</span><span class="sxs-lookup"><span data-stu-id="8fb9e-168">String</span></span>|<span data-ttu-id="8fb9e-169">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8fb9e-170">响应</span><span class="sxs-lookup"><span data-stu-id="8fb9e-170">Response</span></span>
<span data-ttu-id="8fb9e-171">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb9e-172">示例</span><span class="sxs-lookup"><span data-stu-id="8fb9e-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fb9e-173">请求</span><span class="sxs-lookup"><span data-stu-id="8fb9e-173">Request</span></span>
<span data-ttu-id="8fb9e-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="8fb9e-175">响应</span><span class="sxs-lookup"><span data-stu-id="8fb9e-175">Response</span></span>
<span data-ttu-id="8fb9e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8fb9e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






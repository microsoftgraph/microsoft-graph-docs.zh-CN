---
title: 更新 importedAppleDeviceIdentity
description: 更新 importedAppleDeviceIdentity 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4019621eb6f69b288575a592b59b0018582c0b06
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870502"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="c0cb2-103">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c0cb2-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="c0cb2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0cb2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0cb2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0cb2-107">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0cb2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0cb2-108">Prerequisites</span></span>
<span data-ttu-id="c0cb2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c0cb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0cb2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0cb2-111">Permission type</span></span>|<span data-ttu-id="c0cb2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0cb2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0cb2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0cb2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0cb2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0cb2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0cb2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0cb2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0cb2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-116">Not supported.</span></span>|
|<span data-ttu-id="c0cb2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0cb2-117">Application</span></span>|<span data-ttu-id="c0cb2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0cb2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0cb2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="c0cb2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0cb2-120">Request headers</span></span>
|<span data-ttu-id="c0cb2-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0cb2-121">Header</span></span>|<span data-ttu-id="c0cb2-122">值</span><span class="sxs-lookup"><span data-stu-id="c0cb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0cb2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0cb2-123">Authorization</span></span>|<span data-ttu-id="c0cb2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0cb2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0cb2-125">Accept</span></span>|<span data-ttu-id="c0cb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0cb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0cb2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0cb2-127">Request body</span></span>
<span data-ttu-id="c0cb2-128">在请求正文中，提供[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="c0cb2-129">下表显示时创建[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="c0cb2-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0cb2-130">Property</span></span>|<span data-ttu-id="c0cb2-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0cb2-131">Type</span></span>|<span data-ttu-id="c0cb2-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0cb2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0cb2-133">id</span><span class="sxs-lookup"><span data-stu-id="c0cb2-133">id</span></span>|<span data-ttu-id="c0cb2-134">String</span><span class="sxs-lookup"><span data-stu-id="c0cb2-134">String</span></span>|<span data-ttu-id="c0cb2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-135">Key of the entity.</span></span>|
|<span data-ttu-id="c0cb2-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c0cb2-136">serialNumber</span></span>|<span data-ttu-id="c0cb2-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c0cb2-137">String</span></span>|<span data-ttu-id="c0cb2-138">设备序列号</span><span class="sxs-lookup"><span data-stu-id="c0cb2-138">Device serial number</span></span>|
|<span data-ttu-id="c0cb2-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c0cb2-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c0cb2-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c0cb2-140">String</span></span>|<span data-ttu-id="c0cb2-141">注册配置文件 Id 管理打算在下一步注册过程适用于设备</span><span class="sxs-lookup"><span data-stu-id="c0cb2-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="c0cb2-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c0cb2-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c0cb2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0cb2-143">DateTimeOffset</span></span>|<span data-ttu-id="c0cb2-144">时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="c0cb2-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="c0cb2-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c0cb2-145">isSupervised</span></span>|<span data-ttu-id="c0cb2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0cb2-146">Boolean</span></span>|<span data-ttu-id="c0cb2-147">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c0cb2-148">详细信息位于：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="c0cb2-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="c0cb2-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c0cb2-149">discoverySource</span></span>|[<span data-ttu-id="c0cb2-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c0cb2-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="c0cb2-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-151">Apple device discovery source.</span></span> <span data-ttu-id="c0cb2-152">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c0cb2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0cb2-153">createdDateTime</span></span>|<span data-ttu-id="c0cb2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0cb2-154">DateTimeOffset</span></span>|<span data-ttu-id="c0cb2-155">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="c0cb2-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="c0cb2-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0cb2-156">lastContactedDateTime</span></span>|<span data-ttu-id="c0cb2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0cb2-157">DateTimeOffset</span></span>|<span data-ttu-id="c0cb2-158">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="c0cb2-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="c0cb2-159">说明</span><span class="sxs-lookup"><span data-stu-id="c0cb2-159">description</span></span>|<span data-ttu-id="c0cb2-160">字符串</span><span class="sxs-lookup"><span data-stu-id="c0cb2-160">String</span></span>|<span data-ttu-id="c0cb2-161">设备的说明</span><span class="sxs-lookup"><span data-stu-id="c0cb2-161">The description of the device</span></span>|
|<span data-ttu-id="c0cb2-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c0cb2-162">enrollmentState</span></span>|[<span data-ttu-id="c0cb2-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c0cb2-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c0cb2-164">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-164">The state of the device in Intune.</span></span> <span data-ttu-id="c0cb2-165">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c0cb2-166">platform</span><span class="sxs-lookup"><span data-stu-id="c0cb2-166">platform</span></span>|[<span data-ttu-id="c0cb2-167">平台</span><span class="sxs-lookup"><span data-stu-id="c0cb2-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c0cb2-168">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-168">The platform of the Device.</span></span> <span data-ttu-id="c0cb2-169">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0cb2-170">响应</span><span class="sxs-lookup"><span data-stu-id="c0cb2-170">Response</span></span>
<span data-ttu-id="c0cb2-171">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0cb2-172">示例</span><span class="sxs-lookup"><span data-stu-id="c0cb2-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0cb2-173">请求</span><span class="sxs-lookup"><span data-stu-id="c0cb2-173">Request</span></span>
<span data-ttu-id="c0cb2-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 431

{
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="c0cb2-175">响应</span><span class="sxs-lookup"><span data-stu-id="c0cb2-175">Response</span></span>
<span data-ttu-id="c0cb2-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0cb2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```






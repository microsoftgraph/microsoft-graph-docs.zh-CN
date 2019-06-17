---
title: 更新 importedAppleDeviceIdentity
description: 更新 importedAppleDeviceIdentity 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 501a8bb31d5b01b184f4a53bb4f68fbd27661675
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982334"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="95727-103">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="95727-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="95727-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95727-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95727-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95727-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95727-106">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95727-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95727-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95727-107">Prerequisites</span></span>
<span data-ttu-id="95727-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95727-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95727-110">Permission type</span></span>|<span data-ttu-id="95727-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95727-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95727-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95727-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95727-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95727-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95727-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95727-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95727-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95727-115">Not supported.</span></span>|
|<span data-ttu-id="95727-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95727-116">Application</span></span>|<span data-ttu-id="95727-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95727-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95727-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95727-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="95727-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95727-119">Request headers</span></span>
|<span data-ttu-id="95727-120">标头</span><span class="sxs-lookup"><span data-stu-id="95727-120">Header</span></span>|<span data-ttu-id="95727-121">值</span><span class="sxs-lookup"><span data-stu-id="95727-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95727-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95727-122">Authorization</span></span>|<span data-ttu-id="95727-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95727-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95727-124">接受</span><span class="sxs-lookup"><span data-stu-id="95727-124">Accept</span></span>|<span data-ttu-id="95727-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95727-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95727-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95727-126">Request body</span></span>
<span data-ttu-id="95727-127">在请求正文中, 提供[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95727-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="95727-128">下表显示创建[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95727-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="95727-129">属性</span><span class="sxs-lookup"><span data-stu-id="95727-129">Property</span></span>|<span data-ttu-id="95727-130">类型</span><span class="sxs-lookup"><span data-stu-id="95727-130">Type</span></span>|<span data-ttu-id="95727-131">说明</span><span class="sxs-lookup"><span data-stu-id="95727-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95727-132">id</span><span class="sxs-lookup"><span data-stu-id="95727-132">id</span></span>|<span data-ttu-id="95727-133">字符串</span><span class="sxs-lookup"><span data-stu-id="95727-133">String</span></span>|<span data-ttu-id="95727-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95727-134">Key of the entity.</span></span>|
|<span data-ttu-id="95727-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="95727-135">serialNumber</span></span>|<span data-ttu-id="95727-136">String</span><span class="sxs-lookup"><span data-stu-id="95727-136">String</span></span>|<span data-ttu-id="95727-137">设备序列号</span><span class="sxs-lookup"><span data-stu-id="95727-137">Device serial number</span></span>|
|<span data-ttu-id="95727-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="95727-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="95727-139">String</span><span class="sxs-lookup"><span data-stu-id="95727-139">String</span></span>|<span data-ttu-id="95727-140">注册配置文件 Id 管理员打算在下次注册时应用到设备</span><span class="sxs-lookup"><span data-stu-id="95727-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="95727-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="95727-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="95727-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95727-142">DateTimeOffset</span></span>|<span data-ttu-id="95727-143">已将时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="95727-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="95727-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="95727-144">isSupervised</span></span>|<span data-ttu-id="95727-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95727-145">Boolean</span></span>|<span data-ttu-id="95727-146">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="95727-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="95727-147">有关详细信息, 请参阅:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="95727-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="95727-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="95727-148">discoverySource</span></span>|[<span data-ttu-id="95727-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="95727-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="95727-150">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="95727-150">Apple device discovery source.</span></span> <span data-ttu-id="95727-151">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="95727-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="95727-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95727-152">createdDateTime</span></span>|<span data-ttu-id="95727-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95727-153">DateTimeOffset</span></span>|<span data-ttu-id="95727-154">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="95727-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="95727-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="95727-155">lastContactedDateTime</span></span>|<span data-ttu-id="95727-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95727-156">DateTimeOffset</span></span>|<span data-ttu-id="95727-157">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="95727-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="95727-158">说明</span><span class="sxs-lookup"><span data-stu-id="95727-158">description</span></span>|<span data-ttu-id="95727-159">String</span><span class="sxs-lookup"><span data-stu-id="95727-159">String</span></span>|<span data-ttu-id="95727-160">设备的说明</span><span class="sxs-lookup"><span data-stu-id="95727-160">The description of the device</span></span>|
|<span data-ttu-id="95727-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="95727-161">enrollmentState</span></span>|[<span data-ttu-id="95727-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="95727-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="95727-163">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="95727-163">The state of the device in Intune.</span></span> <span data-ttu-id="95727-164">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="95727-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="95727-165">platform</span><span class="sxs-lookup"><span data-stu-id="95727-165">platform</span></span>|[<span data-ttu-id="95727-166">平台</span><span class="sxs-lookup"><span data-stu-id="95727-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="95727-167">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="95727-167">The platform of the Device.</span></span> <span data-ttu-id="95727-168">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="95727-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="95727-169">响应</span><span class="sxs-lookup"><span data-stu-id="95727-169">Response</span></span>
<span data-ttu-id="95727-170">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95727-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95727-171">示例</span><span class="sxs-lookup"><span data-stu-id="95727-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="95727-172">请求</span><span class="sxs-lookup"><span data-stu-id="95727-172">Request</span></span>
<span data-ttu-id="95727-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95727-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="95727-174">响应</span><span class="sxs-lookup"><span data-stu-id="95727-174">Response</span></span>
<span data-ttu-id="95727-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95727-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: 更新 importedAppleDeviceIdentity
description: 更新 importedAppleDeviceIdentity 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b1d6836aa23b32418bed1c2cf19e06f82cc661c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813095"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="a69ab-103">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a69ab-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="a69ab-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a69ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a69ab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a69ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a69ab-106">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a69ab-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a69ab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a69ab-107">Prerequisites</span></span>
<span data-ttu-id="a69ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a69ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69ab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a69ab-110">Permission type</span></span>|<span data-ttu-id="a69ab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a69ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a69ab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a69ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a69ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a69ab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a69ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a69ab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a69ab-115">Not supported.</span></span>|
|<span data-ttu-id="a69ab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a69ab-116">Application</span></span>|<span data-ttu-id="a69ab-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69ab-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a69ab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a69ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a69ab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a69ab-119">Request headers</span></span>
|<span data-ttu-id="a69ab-120">标头</span><span class="sxs-lookup"><span data-stu-id="a69ab-120">Header</span></span>|<span data-ttu-id="a69ab-121">值</span><span class="sxs-lookup"><span data-stu-id="a69ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a69ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a69ab-122">Authorization</span></span>|<span data-ttu-id="a69ab-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a69ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a69ab-124">接受</span><span class="sxs-lookup"><span data-stu-id="a69ab-124">Accept</span></span>|<span data-ttu-id="a69ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a69ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a69ab-126">Request body</span></span>
<span data-ttu-id="a69ab-127">在请求正文中，提供[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a69ab-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="a69ab-128">下表显示创建[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a69ab-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="a69ab-129">属性</span><span class="sxs-lookup"><span data-stu-id="a69ab-129">Property</span></span>|<span data-ttu-id="a69ab-130">类型</span><span class="sxs-lookup"><span data-stu-id="a69ab-130">Type</span></span>|<span data-ttu-id="a69ab-131">说明</span><span class="sxs-lookup"><span data-stu-id="a69ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a69ab-132">id</span><span class="sxs-lookup"><span data-stu-id="a69ab-132">id</span></span>|<span data-ttu-id="a69ab-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a69ab-133">String</span></span>|<span data-ttu-id="a69ab-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a69ab-134">Key of the entity.</span></span>|
|<span data-ttu-id="a69ab-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a69ab-135">serialNumber</span></span>|<span data-ttu-id="a69ab-136">String</span><span class="sxs-lookup"><span data-stu-id="a69ab-136">String</span></span>|<span data-ttu-id="a69ab-137">设备序列号</span><span class="sxs-lookup"><span data-stu-id="a69ab-137">Device serial number</span></span>|
|<span data-ttu-id="a69ab-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="a69ab-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="a69ab-139">String</span><span class="sxs-lookup"><span data-stu-id="a69ab-139">String</span></span>|<span data-ttu-id="a69ab-140">注册配置文件 Id 管理员打算在下次注册时应用到设备</span><span class="sxs-lookup"><span data-stu-id="a69ab-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="a69ab-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="a69ab-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="a69ab-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69ab-142">DateTimeOffset</span></span>|<span data-ttu-id="a69ab-143">已将时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="a69ab-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="a69ab-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a69ab-144">isSupervised</span></span>|<span data-ttu-id="a69ab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a69ab-145">Boolean</span></span>|<span data-ttu-id="a69ab-146">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="a69ab-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="a69ab-147">有关详细信息，请参阅：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="a69ab-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="a69ab-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a69ab-148">discoverySource</span></span>|[<span data-ttu-id="a69ab-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a69ab-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="a69ab-150">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="a69ab-150">Apple device discovery source.</span></span> <span data-ttu-id="a69ab-151">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="a69ab-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="a69ab-152">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a69ab-152">isDeleted</span></span>|<span data-ttu-id="a69ab-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="a69ab-153">Boolean</span></span>|<span data-ttu-id="a69ab-154">指示设备是否已从 Apple Business Manager 中删除</span><span class="sxs-lookup"><span data-stu-id="a69ab-154">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="a69ab-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a69ab-155">createdDateTime</span></span>|<span data-ttu-id="a69ab-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69ab-156">DateTimeOffset</span></span>|<span data-ttu-id="a69ab-157">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="a69ab-157">Created Date Time of the device</span></span>|
|<span data-ttu-id="a69ab-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a69ab-158">lastContactedDateTime</span></span>|<span data-ttu-id="a69ab-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69ab-159">DateTimeOffset</span></span>|<span data-ttu-id="a69ab-160">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="a69ab-160">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a69ab-161">说明</span><span class="sxs-lookup"><span data-stu-id="a69ab-161">description</span></span>|<span data-ttu-id="a69ab-162">String</span><span class="sxs-lookup"><span data-stu-id="a69ab-162">String</span></span>|<span data-ttu-id="a69ab-163">设备的说明</span><span class="sxs-lookup"><span data-stu-id="a69ab-163">The description of the device</span></span>|
|<span data-ttu-id="a69ab-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a69ab-164">enrollmentState</span></span>|[<span data-ttu-id="a69ab-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a69ab-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="a69ab-166">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="a69ab-166">The state of the device in Intune.</span></span> <span data-ttu-id="a69ab-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a69ab-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a69ab-168">platform</span><span class="sxs-lookup"><span data-stu-id="a69ab-168">platform</span></span>|[<span data-ttu-id="a69ab-169">平台</span><span class="sxs-lookup"><span data-stu-id="a69ab-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a69ab-170">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="a69ab-170">The platform of the Device.</span></span> <span data-ttu-id="a69ab-171">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="a69ab-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="a69ab-172">响应</span><span class="sxs-lookup"><span data-stu-id="a69ab-172">Response</span></span>
<span data-ttu-id="a69ab-173">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a69ab-173">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69ab-174">示例</span><span class="sxs-lookup"><span data-stu-id="a69ab-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="a69ab-175">请求</span><span class="sxs-lookup"><span data-stu-id="a69ab-175">Request</span></span>
<span data-ttu-id="a69ab-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a69ab-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 519

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="a69ab-177">响应</span><span class="sxs-lookup"><span data-stu-id="a69ab-177">Response</span></span>
<span data-ttu-id="a69ab-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a69ab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





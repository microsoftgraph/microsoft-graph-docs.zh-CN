---
title: 创建 importedAppleDeviceIdentityResult
description: 创建新的 importedAppleDeviceIdentityResult 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7066f146c910e62b9d5bf107f00fb911890e5da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451167"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="66901-103">创建 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="66901-103">Create importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="66901-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66901-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66901-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66901-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66901-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66901-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66901-107">创建新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66901-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66901-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66901-108">Prerequisites</span></span>
<span data-ttu-id="66901-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66901-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66901-111">Permission type</span></span>|<span data-ttu-id="66901-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66901-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66901-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66901-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66901-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66901-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66901-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66901-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66901-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66901-116">Not supported.</span></span>|
|<span data-ttu-id="66901-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="66901-117">Application</span></span>|<span data-ttu-id="66901-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66901-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66901-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66901-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="66901-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66901-120">Request headers</span></span>
|<span data-ttu-id="66901-121">标头</span><span class="sxs-lookup"><span data-stu-id="66901-121">Header</span></span>|<span data-ttu-id="66901-122">值</span><span class="sxs-lookup"><span data-stu-id="66901-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66901-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66901-123">Authorization</span></span>|<span data-ttu-id="66901-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66901-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66901-125">接受</span><span class="sxs-lookup"><span data-stu-id="66901-125">Accept</span></span>|<span data-ttu-id="66901-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66901-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66901-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66901-127">Request body</span></span>
<span data-ttu-id="66901-128">在请求正文中，提供 importedAppleDeviceIdentityResult 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66901-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="66901-129">下表显示创建 importedAppleDeviceIdentityResult 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66901-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="66901-130">属性</span><span class="sxs-lookup"><span data-stu-id="66901-130">Property</span></span>|<span data-ttu-id="66901-131">类型</span><span class="sxs-lookup"><span data-stu-id="66901-131">Type</span></span>|<span data-ttu-id="66901-132">说明</span><span class="sxs-lookup"><span data-stu-id="66901-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66901-133">id</span><span class="sxs-lookup"><span data-stu-id="66901-133">id</span></span>|<span data-ttu-id="66901-134">字符串</span><span class="sxs-lookup"><span data-stu-id="66901-134">String</span></span>|<span data-ttu-id="66901-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66901-135">Key of the entity.</span></span> <span data-ttu-id="66901-136">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="66901-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="66901-137">serialNumber</span></span>|<span data-ttu-id="66901-138">String</span><span class="sxs-lookup"><span data-stu-id="66901-138">String</span></span>|<span data-ttu-id="66901-139">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备序列号</span><span class="sxs-lookup"><span data-stu-id="66901-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="66901-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="66901-141">String</span><span class="sxs-lookup"><span data-stu-id="66901-141">String</span></span>|<span data-ttu-id="66901-142">注册配置文件 Id 管理员旨在在继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的下一个注册过程中应用于设备</span><span class="sxs-lookup"><span data-stu-id="66901-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="66901-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="66901-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66901-144">DateTimeOffset</span></span>|<span data-ttu-id="66901-145">将时间注册配置文件分配给继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备</span><span class="sxs-lookup"><span data-stu-id="66901-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="66901-146">isSupervised</span></span>|<span data-ttu-id="66901-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="66901-147">Boolean</span></span>|<span data-ttu-id="66901-148">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="66901-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="66901-149">有关详细信息，请https://support.apple.com/en-us/HT202837参阅从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承</span><span class="sxs-lookup"><span data-stu-id="66901-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="66901-150">discoverySource</span></span>|[<span data-ttu-id="66901-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="66901-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="66901-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="66901-152">Apple device discovery source.</span></span> <span data-ttu-id="66901-153">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="66901-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66901-154">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="66901-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="66901-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="66901-155">isDeleted</span></span>|<span data-ttu-id="66901-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="66901-156">Boolean</span></span>|<span data-ttu-id="66901-157">指示是否从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的 Apple Business Manager 中删除设备</span><span class="sxs-lookup"><span data-stu-id="66901-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66901-158">createdDateTime</span></span>|<span data-ttu-id="66901-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66901-159">DateTimeOffset</span></span>|<span data-ttu-id="66901-160">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="66901-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="66901-161">lastContactedDateTime</span></span>|<span data-ttu-id="66901-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66901-162">DateTimeOffset</span></span>|<span data-ttu-id="66901-163">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="66901-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-164">description</span><span class="sxs-lookup"><span data-stu-id="66901-164">description</span></span>|<span data-ttu-id="66901-165">String</span><span class="sxs-lookup"><span data-stu-id="66901-165">String</span></span>|<span data-ttu-id="66901-166">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="66901-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66901-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="66901-167">enrollmentState</span></span>|[<span data-ttu-id="66901-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="66901-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="66901-169">Intune 中的设备的状态继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="66901-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66901-170">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="66901-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="66901-171">platform</span><span class="sxs-lookup"><span data-stu-id="66901-171">platform</span></span>|[<span data-ttu-id="66901-172">平台</span><span class="sxs-lookup"><span data-stu-id="66901-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="66901-173">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="66901-173">The platform of the Device.</span></span> <span data-ttu-id="66901-174">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="66901-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66901-175">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="66901-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="66901-176">状态</span><span class="sxs-lookup"><span data-stu-id="66901-176">status</span></span>|<span data-ttu-id="66901-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="66901-177">Boolean</span></span>|<span data-ttu-id="66901-178">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="66901-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="66901-179">响应</span><span class="sxs-lookup"><span data-stu-id="66901-179">Response</span></span>
<span data-ttu-id="66901-180">如果成功，此方法在响应`201 Created`正文中返回响应代码和[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66901-180">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66901-181">示例</span><span class="sxs-lookup"><span data-stu-id="66901-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="66901-182">请求</span><span class="sxs-lookup"><span data-stu-id="66901-182">Request</span></span>
<span data-ttu-id="66901-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66901-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="66901-184">响应</span><span class="sxs-lookup"><span data-stu-id="66901-184">Response</span></span>
<span data-ttu-id="66901-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66901-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
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
  "platform": "ios",
  "status": true
}
```




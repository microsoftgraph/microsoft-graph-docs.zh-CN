---
title: 创建 importedAppleDeviceIdentityResult
description: 创建新的 importedAppleDeviceIdentityResult 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fb0493c1b693ddb72b648311a9e329e38420a75
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185026"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="bfd53-103">创建 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="bfd53-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="bfd53-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bfd53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfd53-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bfd53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfd53-106">创建新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfd53-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfd53-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfd53-107">Prerequisites</span></span>
<span data-ttu-id="bfd53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfd53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfd53-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfd53-110">Permission type</span></span>|<span data-ttu-id="bfd53-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfd53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfd53-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfd53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bfd53-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd53-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bfd53-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfd53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfd53-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfd53-115">Not supported.</span></span>|
|<span data-ttu-id="bfd53-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfd53-116">Application</span></span>|<span data-ttu-id="bfd53-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd53-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfd53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfd53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="bfd53-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfd53-119">Request headers</span></span>
|<span data-ttu-id="bfd53-120">标头</span><span class="sxs-lookup"><span data-stu-id="bfd53-120">Header</span></span>|<span data-ttu-id="bfd53-121">值</span><span class="sxs-lookup"><span data-stu-id="bfd53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfd53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfd53-122">Authorization</span></span>|<span data-ttu-id="bfd53-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfd53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfd53-124">接受</span><span class="sxs-lookup"><span data-stu-id="bfd53-124">Accept</span></span>|<span data-ttu-id="bfd53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bfd53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfd53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfd53-126">Request body</span></span>
<span data-ttu-id="bfd53-127">在请求正文中，提供 importedAppleDeviceIdentityResult 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfd53-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="bfd53-128">下表显示创建 importedAppleDeviceIdentityResult 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfd53-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="bfd53-129">属性</span><span class="sxs-lookup"><span data-stu-id="bfd53-129">Property</span></span>|<span data-ttu-id="bfd53-130">类型</span><span class="sxs-lookup"><span data-stu-id="bfd53-130">Type</span></span>|<span data-ttu-id="bfd53-131">说明</span><span class="sxs-lookup"><span data-stu-id="bfd53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfd53-132">id</span><span class="sxs-lookup"><span data-stu-id="bfd53-132">id</span></span>|<span data-ttu-id="bfd53-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bfd53-133">String</span></span>|<span data-ttu-id="bfd53-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bfd53-134">Key of the entity.</span></span> <span data-ttu-id="bfd53-135">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bfd53-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="bfd53-136">serialNumber</span></span>|<span data-ttu-id="bfd53-137">String</span><span class="sxs-lookup"><span data-stu-id="bfd53-137">String</span></span>|<span data-ttu-id="bfd53-138">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备序列号</span><span class="sxs-lookup"><span data-stu-id="bfd53-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="bfd53-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="bfd53-140">String</span><span class="sxs-lookup"><span data-stu-id="bfd53-140">String</span></span>|<span data-ttu-id="bfd53-141">注册配置文件 Id 管理员旨在在继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的下一个注册过程中应用于设备</span><span class="sxs-lookup"><span data-stu-id="bfd53-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="bfd53-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="bfd53-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfd53-143">DateTimeOffset</span></span>|<span data-ttu-id="bfd53-144">将时间注册配置文件分配给继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备</span><span class="sxs-lookup"><span data-stu-id="bfd53-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="bfd53-145">isSupervised</span></span>|<span data-ttu-id="bfd53-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfd53-146">Boolean</span></span>|<span data-ttu-id="bfd53-147">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="bfd53-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="bfd53-148">有关详细信息，请https://support.apple.com/en-us/HT202837参阅从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承</span><span class="sxs-lookup"><span data-stu-id="bfd53-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="bfd53-149">discoverySource</span></span>|[<span data-ttu-id="bfd53-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="bfd53-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="bfd53-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="bfd53-151">Apple device discovery source.</span></span> <span data-ttu-id="bfd53-152">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="bfd53-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="bfd53-153">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="bfd53-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="bfd53-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfd53-154">createdDateTime</span></span>|<span data-ttu-id="bfd53-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfd53-155">DateTimeOffset</span></span>|<span data-ttu-id="bfd53-156">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="bfd53-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfd53-157">lastContactedDateTime</span></span>|<span data-ttu-id="bfd53-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfd53-158">DateTimeOffset</span></span>|<span data-ttu-id="bfd53-159">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="bfd53-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-160">说明</span><span class="sxs-lookup"><span data-stu-id="bfd53-160">description</span></span>|<span data-ttu-id="bfd53-161">String</span><span class="sxs-lookup"><span data-stu-id="bfd53-161">String</span></span>|<span data-ttu-id="bfd53-162">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="bfd53-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="bfd53-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bfd53-163">enrollmentState</span></span>|[<span data-ttu-id="bfd53-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bfd53-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="bfd53-165">Intune 中的设备的状态继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="bfd53-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="bfd53-166">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="bfd53-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="bfd53-167">platform</span><span class="sxs-lookup"><span data-stu-id="bfd53-167">platform</span></span>|[<span data-ttu-id="bfd53-168">平台</span><span class="sxs-lookup"><span data-stu-id="bfd53-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="bfd53-169">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="bfd53-169">The platform of the Device.</span></span> <span data-ttu-id="bfd53-170">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="bfd53-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="bfd53-171">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="bfd53-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="bfd53-172">status</span><span class="sxs-lookup"><span data-stu-id="bfd53-172">status</span></span>|<span data-ttu-id="bfd53-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfd53-173">Boolean</span></span>|<span data-ttu-id="bfd53-174">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="bfd53-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="bfd53-175">响应</span><span class="sxs-lookup"><span data-stu-id="bfd53-175">Response</span></span>
<span data-ttu-id="bfd53-176">如果成功，此方法在响应`201 Created`正文中返回响应代码和[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfd53-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfd53-177">示例</span><span class="sxs-lookup"><span data-stu-id="bfd53-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfd53-178">请求</span><span class="sxs-lookup"><span data-stu-id="bfd53-178">Request</span></span>
<span data-ttu-id="bfd53-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfd53-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="bfd53-180">响应</span><span class="sxs-lookup"><span data-stu-id="bfd53-180">Response</span></span>
<span data-ttu-id="bfd53-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfd53-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





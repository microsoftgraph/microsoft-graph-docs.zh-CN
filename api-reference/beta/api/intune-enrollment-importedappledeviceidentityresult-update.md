---
title: 更新 importedAppleDeviceIdentityResult
description: 更新 importedAppleDeviceIdentityResult 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed950585756caca884e52cf5a2526b0136caa862
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356436"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="624f8-103">更新 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="624f8-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="624f8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="624f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="624f8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="624f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="624f8-106">更新[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="624f8-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="624f8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="624f8-107">Prerequisites</span></span>
<span data-ttu-id="624f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="624f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="624f8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="624f8-110">Permission type</span></span>|<span data-ttu-id="624f8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="624f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="624f8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="624f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="624f8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624f8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="624f8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="624f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="624f8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="624f8-115">Not supported.</span></span>|
|<span data-ttu-id="624f8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="624f8-116">Application</span></span>|<span data-ttu-id="624f8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624f8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="624f8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="624f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="624f8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="624f8-119">Request headers</span></span>
|<span data-ttu-id="624f8-120">标头</span><span class="sxs-lookup"><span data-stu-id="624f8-120">Header</span></span>|<span data-ttu-id="624f8-121">值</span><span class="sxs-lookup"><span data-stu-id="624f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="624f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="624f8-122">Authorization</span></span>|<span data-ttu-id="624f8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="624f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="624f8-124">接受</span><span class="sxs-lookup"><span data-stu-id="624f8-124">Accept</span></span>|<span data-ttu-id="624f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="624f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="624f8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="624f8-126">Request body</span></span>
<span data-ttu-id="624f8-127">在请求正文中, 提供[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="624f8-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="624f8-128">下表显示创建[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="624f8-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="624f8-129">属性</span><span class="sxs-lookup"><span data-stu-id="624f8-129">Property</span></span>|<span data-ttu-id="624f8-130">类型</span><span class="sxs-lookup"><span data-stu-id="624f8-130">Type</span></span>|<span data-ttu-id="624f8-131">说明</span><span class="sxs-lookup"><span data-stu-id="624f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="624f8-132">id</span><span class="sxs-lookup"><span data-stu-id="624f8-132">id</span></span>|<span data-ttu-id="624f8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="624f8-133">String</span></span>|<span data-ttu-id="624f8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="624f8-134">Key of the entity.</span></span> <span data-ttu-id="624f8-135">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="624f8-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="624f8-136">serialNumber</span></span>|<span data-ttu-id="624f8-137">String</span><span class="sxs-lookup"><span data-stu-id="624f8-137">String</span></span>|<span data-ttu-id="624f8-138">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备序列号</span><span class="sxs-lookup"><span data-stu-id="624f8-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="624f8-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="624f8-140">String</span><span class="sxs-lookup"><span data-stu-id="624f8-140">String</span></span>|<span data-ttu-id="624f8-141">注册配置文件 Id 管理员旨在在继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的下一个注册过程中应用于设备</span><span class="sxs-lookup"><span data-stu-id="624f8-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="624f8-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="624f8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624f8-143">DateTimeOffset</span></span>|<span data-ttu-id="624f8-144">将时间注册配置文件分配给继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备</span><span class="sxs-lookup"><span data-stu-id="624f8-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="624f8-145">isSupervised</span></span>|<span data-ttu-id="624f8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="624f8-146">Boolean</span></span>|<span data-ttu-id="624f8-147">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="624f8-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="624f8-148">有关详细信息, 请https://support.apple.com/en-us/HT202837参阅从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承</span><span class="sxs-lookup"><span data-stu-id="624f8-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="624f8-149">discoverySource</span></span>|[<span data-ttu-id="624f8-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="624f8-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="624f8-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="624f8-151">Apple device discovery source.</span></span> <span data-ttu-id="624f8-152">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="624f8-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="624f8-153">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="624f8-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="624f8-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="624f8-154">createdDateTime</span></span>|<span data-ttu-id="624f8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624f8-155">DateTimeOffset</span></span>|<span data-ttu-id="624f8-156">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="624f8-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="624f8-157">lastContactedDateTime</span></span>|<span data-ttu-id="624f8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624f8-158">DateTimeOffset</span></span>|<span data-ttu-id="624f8-159">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="624f8-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-160">说明</span><span class="sxs-lookup"><span data-stu-id="624f8-160">description</span></span>|<span data-ttu-id="624f8-161">String</span><span class="sxs-lookup"><span data-stu-id="624f8-161">String</span></span>|<span data-ttu-id="624f8-162">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="624f8-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="624f8-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="624f8-163">enrollmentState</span></span>|[<span data-ttu-id="624f8-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="624f8-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="624f8-165">Intune 中的设备的状态继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="624f8-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="624f8-166">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="624f8-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="624f8-167">platform</span><span class="sxs-lookup"><span data-stu-id="624f8-167">platform</span></span>|[<span data-ttu-id="624f8-168">平台</span><span class="sxs-lookup"><span data-stu-id="624f8-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="624f8-169">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="624f8-169">The platform of the Device.</span></span> <span data-ttu-id="624f8-170">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="624f8-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="624f8-171">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="624f8-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="624f8-172">status</span><span class="sxs-lookup"><span data-stu-id="624f8-172">status</span></span>|<span data-ttu-id="624f8-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="624f8-173">Boolean</span></span>|<span data-ttu-id="624f8-174">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="624f8-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="624f8-175">响应</span><span class="sxs-lookup"><span data-stu-id="624f8-175">Response</span></span>
<span data-ttu-id="624f8-176">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="624f8-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="624f8-177">示例</span><span class="sxs-lookup"><span data-stu-id="624f8-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="624f8-178">请求</span><span class="sxs-lookup"><span data-stu-id="624f8-178">Request</span></span>
<span data-ttu-id="624f8-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="624f8-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="624f8-180">响应</span><span class="sxs-lookup"><span data-stu-id="624f8-180">Response</span></span>
<span data-ttu-id="624f8-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="624f8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







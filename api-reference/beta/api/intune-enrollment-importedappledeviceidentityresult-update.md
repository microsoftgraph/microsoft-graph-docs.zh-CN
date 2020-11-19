---
title: 更新 importedAppleDeviceIdentityResult
description: 更新 importedAppleDeviceIdentityResult 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4003fd13bb60fa7626a49953d9fa369a9b34b855
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309437"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="c67cf-103">更新 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="c67cf-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="c67cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c67cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c67cf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c67cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c67cf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c67cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c67cf-107">更新 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c67cf-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c67cf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c67cf-108">Prerequisites</span></span>
<span data-ttu-id="c67cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c67cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c67cf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c67cf-111">Permission type</span></span>|<span data-ttu-id="c67cf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c67cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c67cf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c67cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c67cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c67cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c67cf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c67cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c67cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c67cf-116">Not supported.</span></span>|
|<span data-ttu-id="c67cf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c67cf-117">Application</span></span>|<span data-ttu-id="c67cf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c67cf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c67cf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c67cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="c67cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c67cf-120">Request headers</span></span>
|<span data-ttu-id="c67cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="c67cf-121">Header</span></span>|<span data-ttu-id="c67cf-122">值</span><span class="sxs-lookup"><span data-stu-id="c67cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c67cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c67cf-123">Authorization</span></span>|<span data-ttu-id="c67cf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c67cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c67cf-125">接受</span><span class="sxs-lookup"><span data-stu-id="c67cf-125">Accept</span></span>|<span data-ttu-id="c67cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c67cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c67cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c67cf-127">Request body</span></span>
<span data-ttu-id="c67cf-128">在请求正文中，提供 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c67cf-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="c67cf-129">下表显示创建 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c67cf-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="c67cf-130">属性</span><span class="sxs-lookup"><span data-stu-id="c67cf-130">Property</span></span>|<span data-ttu-id="c67cf-131">类型</span><span class="sxs-lookup"><span data-stu-id="c67cf-131">Type</span></span>|<span data-ttu-id="c67cf-132">说明</span><span class="sxs-lookup"><span data-stu-id="c67cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67cf-133">id</span><span class="sxs-lookup"><span data-stu-id="c67cf-133">id</span></span>|<span data-ttu-id="c67cf-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c67cf-134">String</span></span>|<span data-ttu-id="c67cf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c67cf-135">Key of the entity.</span></span> <span data-ttu-id="c67cf-136">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c67cf-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c67cf-137">serialNumber</span></span>|<span data-ttu-id="c67cf-138">String</span><span class="sxs-lookup"><span data-stu-id="c67cf-138">String</span></span>|<span data-ttu-id="c67cf-139">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备序列号</span><span class="sxs-lookup"><span data-stu-id="c67cf-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c67cf-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c67cf-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c67cf-141">String</span></span>|<span data-ttu-id="c67cf-142">注册配置文件 Id 管理员旨在在继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的下一个注册过程中应用于设备</span><span class="sxs-lookup"><span data-stu-id="c67cf-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c67cf-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c67cf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67cf-144">DateTimeOffset</span></span>|<span data-ttu-id="c67cf-145">将时间注册配置文件分配给继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备</span><span class="sxs-lookup"><span data-stu-id="c67cf-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c67cf-146">isSupervised</span></span>|<span data-ttu-id="c67cf-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c67cf-147">Boolean</span></span>|<span data-ttu-id="c67cf-148">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="c67cf-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c67cf-149">有关详细信息，请参阅 https://support.apple.com/HT202837 从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承</span><span class="sxs-lookup"><span data-stu-id="c67cf-149">More information is at: https://support.apple.com/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c67cf-150">discoverySource</span></span>|[<span data-ttu-id="c67cf-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c67cf-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="c67cf-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="c67cf-152">Apple device discovery source.</span></span> <span data-ttu-id="c67cf-153">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="c67cf-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c67cf-154">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="c67cf-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c67cf-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c67cf-155">isDeleted</span></span>|<span data-ttu-id="c67cf-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c67cf-156">Boolean</span></span>|<span data-ttu-id="c67cf-157">指示是否从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的 Apple Business Manager 中删除设备</span><span class="sxs-lookup"><span data-stu-id="c67cf-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c67cf-158">createdDateTime</span></span>|<span data-ttu-id="c67cf-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67cf-159">DateTimeOffset</span></span>|<span data-ttu-id="c67cf-160">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="c67cf-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c67cf-161">lastContactedDateTime</span></span>|<span data-ttu-id="c67cf-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67cf-162">DateTimeOffset</span></span>|<span data-ttu-id="c67cf-163">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="c67cf-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-164">description</span><span class="sxs-lookup"><span data-stu-id="c67cf-164">description</span></span>|<span data-ttu-id="c67cf-165">字符串</span><span class="sxs-lookup"><span data-stu-id="c67cf-165">String</span></span>|<span data-ttu-id="c67cf-166">从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="c67cf-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c67cf-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c67cf-167">enrollmentState</span></span>|[<span data-ttu-id="c67cf-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c67cf-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="c67cf-169">Intune 中的设备的状态继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="c67cf-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c67cf-170">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c67cf-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c67cf-171">平台</span><span class="sxs-lookup"><span data-stu-id="c67cf-171">platform</span></span>|[<span data-ttu-id="c67cf-172">平台</span><span class="sxs-lookup"><span data-stu-id="c67cf-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c67cf-173">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="c67cf-173">The platform of the Device.</span></span> <span data-ttu-id="c67cf-174">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="c67cf-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c67cf-175">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="c67cf-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="c67cf-176">status</span><span class="sxs-lookup"><span data-stu-id="c67cf-176">status</span></span>|<span data-ttu-id="c67cf-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="c67cf-177">Boolean</span></span>|<span data-ttu-id="c67cf-178">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="c67cf-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="c67cf-179">响应</span><span class="sxs-lookup"><span data-stu-id="c67cf-179">Response</span></span>
<span data-ttu-id="c67cf-180">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c67cf-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c67cf-181">示例</span><span class="sxs-lookup"><span data-stu-id="c67cf-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="c67cf-182">请求</span><span class="sxs-lookup"><span data-stu-id="c67cf-182">Request</span></span>
<span data-ttu-id="c67cf-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c67cf-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="c67cf-184">响应</span><span class="sxs-lookup"><span data-stu-id="c67cf-184">Response</span></span>
<span data-ttu-id="c67cf-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c67cf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





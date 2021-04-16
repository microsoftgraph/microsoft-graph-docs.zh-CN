---
title: 更新 importedAppleDeviceIdentityResult
description: 更新 importedAppleDeviceIdentityResult 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f0db5a3ed08c54e7036e82a22f9e5658aa04ace
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868202"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="9e6e1-103">更新 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="9e6e1-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="9e6e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e6e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e6e1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e6e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e6e1-107">更新 [importedAppleDeviceIdentityResult 对象](../resources/intune-enrollment-importedappledeviceidentityresult.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e6e1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e6e1-108">Prerequisites</span></span>
<span data-ttu-id="9e6e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e6e1-111">Permission type</span></span>|<span data-ttu-id="9e6e1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e6e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e6e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e6e1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6e1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9e6e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e6e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e6e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-116">Not supported.</span></span>|
|<span data-ttu-id="9e6e1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e6e1-117">Application</span></span>|<span data-ttu-id="9e6e1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6e1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e6e1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e6e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="9e6e1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e6e1-120">Request headers</span></span>
|<span data-ttu-id="9e6e1-121">标头</span><span class="sxs-lookup"><span data-stu-id="9e6e1-121">Header</span></span>|<span data-ttu-id="9e6e1-122">值</span><span class="sxs-lookup"><span data-stu-id="9e6e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e6e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e6e1-123">Authorization</span></span>|<span data-ttu-id="9e6e1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e6e1-125">接受</span><span class="sxs-lookup"><span data-stu-id="9e6e1-125">Accept</span></span>|<span data-ttu-id="9e6e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e6e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e6e1-127">Request body</span></span>
<span data-ttu-id="9e6e1-128">在请求正文中，提供 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="9e6e1-129">下表显示创建 [importedAppleDeviceIdentityResult 时所需的属性](../resources/intune-enrollment-importedappledeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="9e6e1-130">属性</span><span class="sxs-lookup"><span data-stu-id="9e6e1-130">Property</span></span>|<span data-ttu-id="9e6e1-131">类型</span><span class="sxs-lookup"><span data-stu-id="9e6e1-131">Type</span></span>|<span data-ttu-id="9e6e1-132">说明</span><span class="sxs-lookup"><span data-stu-id="9e6e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e6e1-133">id</span><span class="sxs-lookup"><span data-stu-id="9e6e1-133">id</span></span>|<span data-ttu-id="9e6e1-134">String</span><span class="sxs-lookup"><span data-stu-id="9e6e1-134">String</span></span>|<span data-ttu-id="9e6e1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-135">Key of the entity.</span></span> <span data-ttu-id="9e6e1-136">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9e6e1-137">serialNumber</span></span>|<span data-ttu-id="9e6e1-138">String</span><span class="sxs-lookup"><span data-stu-id="9e6e1-138">String</span></span>|<span data-ttu-id="9e6e1-139">设备序列号 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="9e6e1-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="9e6e1-141">String</span><span class="sxs-lookup"><span data-stu-id="9e6e1-141">String</span></span>|<span data-ttu-id="9e6e1-142">注册配置文件 ID 管理员打算在下一次注册期间应用到设备 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6e1-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="9e6e1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6e1-144">DateTimeOffset</span></span>|<span data-ttu-id="9e6e1-145">向设备分配注册配置文件的时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9e6e1-146">isSupervised</span></span>|<span data-ttu-id="9e6e1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e6e1-147">Boolean</span></span>|<span data-ttu-id="9e6e1-148">指示 Apple 设备是否受监督。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="9e6e1-149">详细信息位于： https://support.apple.com/en-us/HT202837 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9e6e1-150">discoverySource</span></span>|[<span data-ttu-id="9e6e1-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9e6e1-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="9e6e1-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-152">Apple device discovery source.</span></span> <span data-ttu-id="9e6e1-153">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="9e6e1-154">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="9e6e1-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9e6e1-155">isDeleted</span></span>|<span data-ttu-id="9e6e1-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e6e1-156">Boolean</span></span>|<span data-ttu-id="9e6e1-157">指示设备是否从 Apple Business Manager 中删除 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6e1-158">createdDateTime</span></span>|<span data-ttu-id="9e6e1-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6e1-159">DateTimeOffset</span></span>|<span data-ttu-id="9e6e1-160">设备的创建日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6e1-161">lastContactedDateTime</span></span>|<span data-ttu-id="9e6e1-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6e1-162">DateTimeOffset</span></span>|<span data-ttu-id="9e6e1-163">设备的上次联系日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-164">说明</span><span class="sxs-lookup"><span data-stu-id="9e6e1-164">description</span></span>|<span data-ttu-id="9e6e1-165">String</span><span class="sxs-lookup"><span data-stu-id="9e6e1-165">String</span></span>|<span data-ttu-id="9e6e1-166">设备描述 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9e6e1-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="9e6e1-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9e6e1-167">enrollmentState</span></span>|[<span data-ttu-id="9e6e1-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9e6e1-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="9e6e1-169">Intune 中的设备状态 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="9e6e1-170">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="9e6e1-171">平台</span><span class="sxs-lookup"><span data-stu-id="9e6e1-171">platform</span></span>|[<span data-ttu-id="9e6e1-172">平台</span><span class="sxs-lookup"><span data-stu-id="9e6e1-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="9e6e1-173">设备平台。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-173">The platform of the Device.</span></span> <span data-ttu-id="9e6e1-174">继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="9e6e1-175">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="9e6e1-176">状态</span><span class="sxs-lookup"><span data-stu-id="9e6e1-176">status</span></span>|<span data-ttu-id="9e6e1-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e6e1-177">Boolean</span></span>|<span data-ttu-id="9e6e1-178">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="9e6e1-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="9e6e1-179">响应</span><span class="sxs-lookup"><span data-stu-id="9e6e1-179">Response</span></span>
<span data-ttu-id="9e6e1-180">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e6e1-181">示例</span><span class="sxs-lookup"><span data-stu-id="9e6e1-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e6e1-182">请求</span><span class="sxs-lookup"><span data-stu-id="9e6e1-182">Request</span></span>
<span data-ttu-id="9e6e1-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e6e1-184">响应</span><span class="sxs-lookup"><span data-stu-id="9e6e1-184">Response</span></span>
<span data-ttu-id="9e6e1-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e6e1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





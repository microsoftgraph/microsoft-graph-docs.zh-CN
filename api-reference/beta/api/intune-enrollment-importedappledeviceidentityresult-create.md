---
title: 创建 importedAppleDeviceIdentityResult
description: 创建新的 importedAppleDeviceIdentityResult 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd48716e7268997305a5b8840beacbab9106cf42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417726"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="5f439-103">创建 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="5f439-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="5f439-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5f439-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f439-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f439-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f439-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f439-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f439-107">创建新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f439-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f439-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f439-108">Prerequisites</span></span>
<span data-ttu-id="5f439-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f439-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f439-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f439-111">Permission type</span></span>|<span data-ttu-id="5f439-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f439-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f439-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f439-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f439-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f439-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f439-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f439-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f439-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f439-116">Not supported.</span></span>|
|<span data-ttu-id="5f439-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f439-117">Application</span></span>|<span data-ttu-id="5f439-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f439-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f439-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f439-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="5f439-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f439-120">Request headers</span></span>
|<span data-ttu-id="5f439-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f439-121">Header</span></span>|<span data-ttu-id="5f439-122">值</span><span class="sxs-lookup"><span data-stu-id="5f439-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f439-123">授权</span><span class="sxs-lookup"><span data-stu-id="5f439-123">Authorization</span></span>|<span data-ttu-id="5f439-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f439-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f439-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f439-125">Accept</span></span>|<span data-ttu-id="5f439-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f439-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f439-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f439-127">Request body</span></span>
<span data-ttu-id="5f439-128">在请求正文中，提供 importedAppleDeviceIdentityResult 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f439-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="5f439-129">下表显示时创建 importedAppleDeviceIdentityResult 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5f439-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="5f439-130">属性</span><span class="sxs-lookup"><span data-stu-id="5f439-130">Property</span></span>|<span data-ttu-id="5f439-131">类型</span><span class="sxs-lookup"><span data-stu-id="5f439-131">Type</span></span>|<span data-ttu-id="5f439-132">说明</span><span class="sxs-lookup"><span data-stu-id="5f439-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f439-133">id</span><span class="sxs-lookup"><span data-stu-id="5f439-133">id</span></span>|<span data-ttu-id="5f439-134">String</span><span class="sxs-lookup"><span data-stu-id="5f439-134">String</span></span>|<span data-ttu-id="5f439-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5f439-135">Key of the entity.</span></span> <span data-ttu-id="5f439-136">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5f439-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5f439-137">serialNumber</span></span>|<span data-ttu-id="5f439-138">String</span><span class="sxs-lookup"><span data-stu-id="5f439-138">String</span></span>|<span data-ttu-id="5f439-139">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备序列号继承</span><span class="sxs-lookup"><span data-stu-id="5f439-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="5f439-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="5f439-141">String</span><span class="sxs-lookup"><span data-stu-id="5f439-141">String</span></span>|<span data-ttu-id="5f439-142">注册配置文件 Id 管理打算在下一步注册继承过程中从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)适用于设备</span><span class="sxs-lookup"><span data-stu-id="5f439-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="5f439-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="5f439-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f439-144">DateTimeOffset</span></span>|<span data-ttu-id="5f439-145">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)时间注册配置文件分配给设备继承</span><span class="sxs-lookup"><span data-stu-id="5f439-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5f439-146">isSupervised</span></span>|<span data-ttu-id="5f439-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f439-147">Boolean</span></span>|<span data-ttu-id="5f439-148">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="5f439-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="5f439-149">详细信息位于：https://support.apple.com/en-us/HT202837继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5f439-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5f439-150">discoverySource</span></span>|[<span data-ttu-id="5f439-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5f439-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="5f439-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="5f439-152">Apple device discovery source.</span></span> <span data-ttu-id="5f439-153">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="5f439-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5f439-154">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="5f439-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="5f439-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f439-155">createdDateTime</span></span>|<span data-ttu-id="5f439-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f439-156">DateTimeOffset</span></span>|<span data-ttu-id="5f439-157">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)创建设备继承的日期时间</span><span class="sxs-lookup"><span data-stu-id="5f439-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f439-158">lastContactedDateTime</span></span>|<span data-ttu-id="5f439-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f439-159">DateTimeOffset</span></span>|<span data-ttu-id="5f439-160">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="5f439-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-161">说明</span><span class="sxs-lookup"><span data-stu-id="5f439-161">description</span></span>|<span data-ttu-id="5f439-162">String</span><span class="sxs-lookup"><span data-stu-id="5f439-162">String</span></span>|<span data-ttu-id="5f439-163">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承说明</span><span class="sxs-lookup"><span data-stu-id="5f439-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5f439-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5f439-164">enrollmentState</span></span>|[<span data-ttu-id="5f439-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5f439-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5f439-166">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)中 Intune 继承的设备的状态。</span><span class="sxs-lookup"><span data-stu-id="5f439-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5f439-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="5f439-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5f439-168">platform</span><span class="sxs-lookup"><span data-stu-id="5f439-168">platform</span></span>|[<span data-ttu-id="5f439-169">平台</span><span class="sxs-lookup"><span data-stu-id="5f439-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5f439-170">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="5f439-170">The platform of the Device.</span></span> <span data-ttu-id="5f439-171">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="5f439-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5f439-172">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="5f439-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="5f439-173">status</span><span class="sxs-lookup"><span data-stu-id="5f439-173">status</span></span>|<span data-ttu-id="5f439-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f439-174">Boolean</span></span>|<span data-ttu-id="5f439-175">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="5f439-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="5f439-176">响应</span><span class="sxs-lookup"><span data-stu-id="5f439-176">Response</span></span>
<span data-ttu-id="5f439-177">如果成功，此方法返回`201 Created`响应代码和响应正文中的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f439-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f439-178">示例</span><span class="sxs-lookup"><span data-stu-id="5f439-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f439-179">请求</span><span class="sxs-lookup"><span data-stu-id="5f439-179">Request</span></span>
<span data-ttu-id="5f439-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f439-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f439-181">响应</span><span class="sxs-lookup"><span data-stu-id="5f439-181">Response</span></span>
<span data-ttu-id="5f439-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f439-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





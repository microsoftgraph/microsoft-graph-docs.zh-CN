---
title: 更新 importedAppleDeviceIdentityResult
description: 更新 importedAppleDeviceIdentityResult 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 434bc2f19e708041b93ff79a8708f30bed086855
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915492"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="0564e-103">更新 importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="0564e-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="0564e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0564e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0564e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0564e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0564e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0564e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0564e-107">更新[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0564e-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0564e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0564e-108">Prerequisites</span></span>
<span data-ttu-id="0564e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0564e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0564e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0564e-111">Permission type</span></span>|<span data-ttu-id="0564e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0564e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0564e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0564e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0564e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0564e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0564e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0564e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0564e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0564e-116">Not supported.</span></span>|
|<span data-ttu-id="0564e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0564e-117">Application</span></span>|<span data-ttu-id="0564e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0564e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0564e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0564e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0564e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0564e-120">Request headers</span></span>
|<span data-ttu-id="0564e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0564e-121">Header</span></span>|<span data-ttu-id="0564e-122">值</span><span class="sxs-lookup"><span data-stu-id="0564e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0564e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0564e-123">Authorization</span></span>|<span data-ttu-id="0564e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0564e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0564e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0564e-125">Accept</span></span>|<span data-ttu-id="0564e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0564e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0564e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0564e-127">Request body</span></span>
<span data-ttu-id="0564e-128">在请求正文中，提供[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0564e-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="0564e-129">下表显示时创建[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0564e-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="0564e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0564e-130">Property</span></span>|<span data-ttu-id="0564e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0564e-131">Type</span></span>|<span data-ttu-id="0564e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0564e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0564e-133">id</span><span class="sxs-lookup"><span data-stu-id="0564e-133">id</span></span>|<span data-ttu-id="0564e-134">String</span><span class="sxs-lookup"><span data-stu-id="0564e-134">String</span></span>|<span data-ttu-id="0564e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0564e-135">Key of the entity.</span></span> <span data-ttu-id="0564e-136">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0564e-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0564e-137">serialNumber</span></span>|<span data-ttu-id="0564e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="0564e-138">String</span></span>|<span data-ttu-id="0564e-139">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备序列号继承</span><span class="sxs-lookup"><span data-stu-id="0564e-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="0564e-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="0564e-141">字符串</span><span class="sxs-lookup"><span data-stu-id="0564e-141">String</span></span>|<span data-ttu-id="0564e-142">注册配置文件 Id 管理打算在下一步注册继承过程中从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)适用于设备</span><span class="sxs-lookup"><span data-stu-id="0564e-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="0564e-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="0564e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0564e-144">DateTimeOffset</span></span>|<span data-ttu-id="0564e-145">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)时间注册配置文件分配给设备继承</span><span class="sxs-lookup"><span data-stu-id="0564e-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0564e-146">isSupervised</span></span>|<span data-ttu-id="0564e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0564e-147">Boolean</span></span>|<span data-ttu-id="0564e-148">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="0564e-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="0564e-149">详细信息位于：https://support.apple.com/en-us/HT202837继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0564e-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0564e-150">discoverySource</span></span>|[<span data-ttu-id="0564e-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0564e-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="0564e-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="0564e-152">Apple device discovery source.</span></span> <span data-ttu-id="0564e-153">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="0564e-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0564e-154">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="0564e-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="0564e-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0564e-155">createdDateTime</span></span>|<span data-ttu-id="0564e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0564e-156">DateTimeOffset</span></span>|<span data-ttu-id="0564e-157">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)创建设备继承的日期时间</span><span class="sxs-lookup"><span data-stu-id="0564e-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="0564e-158">lastContactedDateTime</span></span>|<span data-ttu-id="0564e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0564e-159">DateTimeOffset</span></span>|<span data-ttu-id="0564e-160">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="0564e-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-161">说明</span><span class="sxs-lookup"><span data-stu-id="0564e-161">description</span></span>|<span data-ttu-id="0564e-162">字符串</span><span class="sxs-lookup"><span data-stu-id="0564e-162">String</span></span>|<span data-ttu-id="0564e-163">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承说明</span><span class="sxs-lookup"><span data-stu-id="0564e-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0564e-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0564e-164">enrollmentState</span></span>|[<span data-ttu-id="0564e-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0564e-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="0564e-166">从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)中 Intune 继承的设备的状态。</span><span class="sxs-lookup"><span data-stu-id="0564e-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0564e-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="0564e-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0564e-168">platform</span><span class="sxs-lookup"><span data-stu-id="0564e-168">platform</span></span>|[<span data-ttu-id="0564e-169">平台</span><span class="sxs-lookup"><span data-stu-id="0564e-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="0564e-170">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="0564e-170">The platform of the Device.</span></span> <span data-ttu-id="0564e-171">继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="0564e-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0564e-172">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="0564e-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="0564e-173">status</span><span class="sxs-lookup"><span data-stu-id="0564e-173">status</span></span>|<span data-ttu-id="0564e-174">布尔</span><span class="sxs-lookup"><span data-stu-id="0564e-174">Boolean</span></span>|<span data-ttu-id="0564e-175">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="0564e-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="0564e-176">响应</span><span class="sxs-lookup"><span data-stu-id="0564e-176">Response</span></span>
<span data-ttu-id="0564e-177">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0564e-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0564e-178">示例</span><span class="sxs-lookup"><span data-stu-id="0564e-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="0564e-179">请求</span><span class="sxs-lookup"><span data-stu-id="0564e-179">Request</span></span>
<span data-ttu-id="0564e-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0564e-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 450

{
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

### <a name="response"></a><span data-ttu-id="0564e-181">响应</span><span class="sxs-lookup"><span data-stu-id="0564e-181">Response</span></span>
<span data-ttu-id="0564e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0564e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






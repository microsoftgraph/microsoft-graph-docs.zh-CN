---
title: 创建 importedAppleDeviceIdentity
description: 创建新的 importedAppleDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3cad7ae4eba432bfd211864962c4213ece53dd3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726778"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="88385-103">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="88385-103">Create importedAppleDeviceIdentity</span></span>

<span data-ttu-id="88385-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88385-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88385-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88385-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88385-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88385-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88385-107">创建新的 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88385-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88385-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88385-108">Prerequisites</span></span>
<span data-ttu-id="88385-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88385-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88385-111">Permission type</span></span>|<span data-ttu-id="88385-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88385-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88385-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88385-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88385-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88385-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88385-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88385-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88385-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88385-116">Not supported.</span></span>|
|<span data-ttu-id="88385-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88385-117">Application</span></span>|<span data-ttu-id="88385-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88385-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88385-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88385-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="88385-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88385-120">Request headers</span></span>
|<span data-ttu-id="88385-121">标头</span><span class="sxs-lookup"><span data-stu-id="88385-121">Header</span></span>|<span data-ttu-id="88385-122">值</span><span class="sxs-lookup"><span data-stu-id="88385-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88385-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88385-123">Authorization</span></span>|<span data-ttu-id="88385-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88385-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88385-125">接受</span><span class="sxs-lookup"><span data-stu-id="88385-125">Accept</span></span>|<span data-ttu-id="88385-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88385-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88385-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88385-127">Request body</span></span>
<span data-ttu-id="88385-128">在请求正文中，提供 importedAppleDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88385-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="88385-129">下表显示创建 importedAppleDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88385-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="88385-130">属性</span><span class="sxs-lookup"><span data-stu-id="88385-130">Property</span></span>|<span data-ttu-id="88385-131">类型</span><span class="sxs-lookup"><span data-stu-id="88385-131">Type</span></span>|<span data-ttu-id="88385-132">说明</span><span class="sxs-lookup"><span data-stu-id="88385-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88385-133">id</span><span class="sxs-lookup"><span data-stu-id="88385-133">id</span></span>|<span data-ttu-id="88385-134">String</span><span class="sxs-lookup"><span data-stu-id="88385-134">String</span></span>|<span data-ttu-id="88385-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88385-135">Key of the entity.</span></span>|
|<span data-ttu-id="88385-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="88385-136">serialNumber</span></span>|<span data-ttu-id="88385-137">String</span><span class="sxs-lookup"><span data-stu-id="88385-137">String</span></span>|<span data-ttu-id="88385-138">设备序列号</span><span class="sxs-lookup"><span data-stu-id="88385-138">Device serial number</span></span>|
|<span data-ttu-id="88385-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="88385-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="88385-140">String</span><span class="sxs-lookup"><span data-stu-id="88385-140">String</span></span>|<span data-ttu-id="88385-141">注册配置文件 Id 管理员打算在下次注册时应用到设备</span><span class="sxs-lookup"><span data-stu-id="88385-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="88385-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="88385-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="88385-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88385-143">DateTimeOffset</span></span>|<span data-ttu-id="88385-144">已将时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="88385-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="88385-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="88385-145">isSupervised</span></span>|<span data-ttu-id="88385-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="88385-146">Boolean</span></span>|<span data-ttu-id="88385-147">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="88385-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="88385-148">有关详细信息，请参阅： https://support.apple.com/HT202837</span><span class="sxs-lookup"><span data-stu-id="88385-148">More information is at: https://support.apple.com/HT202837</span></span>|
|<span data-ttu-id="88385-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="88385-149">discoverySource</span></span>|[<span data-ttu-id="88385-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="88385-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="88385-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="88385-151">Apple device discovery source.</span></span> <span data-ttu-id="88385-152">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="88385-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="88385-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="88385-153">isDeleted</span></span>|<span data-ttu-id="88385-154">布尔</span><span class="sxs-lookup"><span data-stu-id="88385-154">Boolean</span></span>|<span data-ttu-id="88385-155">指示设备是否已从 Apple Business Manager 中删除</span><span class="sxs-lookup"><span data-stu-id="88385-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="88385-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88385-156">createdDateTime</span></span>|<span data-ttu-id="88385-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88385-157">DateTimeOffset</span></span>|<span data-ttu-id="88385-158">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="88385-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="88385-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="88385-159">lastContactedDateTime</span></span>|<span data-ttu-id="88385-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88385-160">DateTimeOffset</span></span>|<span data-ttu-id="88385-161">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="88385-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="88385-162">说明</span><span class="sxs-lookup"><span data-stu-id="88385-162">description</span></span>|<span data-ttu-id="88385-163">String</span><span class="sxs-lookup"><span data-stu-id="88385-163">String</span></span>|<span data-ttu-id="88385-164">设备的说明</span><span class="sxs-lookup"><span data-stu-id="88385-164">The description of the device</span></span>|
|<span data-ttu-id="88385-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="88385-165">enrollmentState</span></span>|[<span data-ttu-id="88385-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="88385-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="88385-167">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="88385-167">The state of the device in Intune.</span></span> <span data-ttu-id="88385-168">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="88385-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="88385-169">平台</span><span class="sxs-lookup"><span data-stu-id="88385-169">platform</span></span>|[<span data-ttu-id="88385-170">平台</span><span class="sxs-lookup"><span data-stu-id="88385-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="88385-171">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="88385-171">The platform of the Device.</span></span> <span data-ttu-id="88385-172">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="88385-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="88385-173">响应</span><span class="sxs-lookup"><span data-stu-id="88385-173">Response</span></span>
<span data-ttu-id="88385-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88385-174">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88385-175">示例</span><span class="sxs-lookup"><span data-stu-id="88385-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="88385-176">请求</span><span class="sxs-lookup"><span data-stu-id="88385-176">Request</span></span>
<span data-ttu-id="88385-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88385-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="88385-178">响应</span><span class="sxs-lookup"><span data-stu-id="88385-178">Response</span></span>
<span data-ttu-id="88385-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88385-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






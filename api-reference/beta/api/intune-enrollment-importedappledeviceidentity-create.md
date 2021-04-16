---
title: 创建 importedAppleDeviceIdentity
description: 创建新的 importedAppleDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8fa76a6c4a9138ae406322c1060552992ff0b3e7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867012"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="08fd4-103">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="08fd4-103">Create importedAppleDeviceIdentity</span></span>

<span data-ttu-id="08fd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08fd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08fd4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08fd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08fd4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08fd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08fd4-107">创建新的 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08fd4-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08fd4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08fd4-108">Prerequisites</span></span>
<span data-ttu-id="08fd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08fd4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08fd4-111">Permission type</span></span>|<span data-ttu-id="08fd4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08fd4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08fd4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08fd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08fd4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fd4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08fd4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08fd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08fd4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08fd4-116">Not supported.</span></span>|
|<span data-ttu-id="08fd4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08fd4-117">Application</span></span>|<span data-ttu-id="08fd4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fd4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08fd4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08fd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="08fd4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08fd4-120">Request headers</span></span>
|<span data-ttu-id="08fd4-121">标头</span><span class="sxs-lookup"><span data-stu-id="08fd4-121">Header</span></span>|<span data-ttu-id="08fd4-122">值</span><span class="sxs-lookup"><span data-stu-id="08fd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08fd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08fd4-123">Authorization</span></span>|<span data-ttu-id="08fd4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08fd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08fd4-125">接受</span><span class="sxs-lookup"><span data-stu-id="08fd4-125">Accept</span></span>|<span data-ttu-id="08fd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08fd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fd4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08fd4-127">Request body</span></span>
<span data-ttu-id="08fd4-128">在请求正文中，提供 importedAppleDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08fd4-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="08fd4-129">下表显示创建 importedAppleDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08fd4-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="08fd4-130">属性</span><span class="sxs-lookup"><span data-stu-id="08fd4-130">Property</span></span>|<span data-ttu-id="08fd4-131">类型</span><span class="sxs-lookup"><span data-stu-id="08fd4-131">Type</span></span>|<span data-ttu-id="08fd4-132">说明</span><span class="sxs-lookup"><span data-stu-id="08fd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fd4-133">id</span><span class="sxs-lookup"><span data-stu-id="08fd4-133">id</span></span>|<span data-ttu-id="08fd4-134">String</span><span class="sxs-lookup"><span data-stu-id="08fd4-134">String</span></span>|<span data-ttu-id="08fd4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="08fd4-135">Key of the entity.</span></span>|
|<span data-ttu-id="08fd4-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="08fd4-136">serialNumber</span></span>|<span data-ttu-id="08fd4-137">String</span><span class="sxs-lookup"><span data-stu-id="08fd4-137">String</span></span>|<span data-ttu-id="08fd4-138">设备序列号</span><span class="sxs-lookup"><span data-stu-id="08fd4-138">Device serial number</span></span>|
|<span data-ttu-id="08fd4-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="08fd4-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="08fd4-140">String</span><span class="sxs-lookup"><span data-stu-id="08fd4-140">String</span></span>|<span data-ttu-id="08fd4-141">注册配置文件 ID 管理员打算在下一次注册期间应用到设备</span><span class="sxs-lookup"><span data-stu-id="08fd4-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="08fd4-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="08fd4-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="08fd4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fd4-143">DateTimeOffset</span></span>|<span data-ttu-id="08fd4-144">向设备分配注册配置文件的时间</span><span class="sxs-lookup"><span data-stu-id="08fd4-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="08fd4-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="08fd4-145">isSupervised</span></span>|<span data-ttu-id="08fd4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08fd4-146">Boolean</span></span>|<span data-ttu-id="08fd4-147">指示 Apple 设备是否受监督。</span><span class="sxs-lookup"><span data-stu-id="08fd4-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="08fd4-148">有关详细信息，请参阅： https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="08fd4-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="08fd4-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="08fd4-149">discoverySource</span></span>|[<span data-ttu-id="08fd4-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="08fd4-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="08fd4-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="08fd4-151">Apple device discovery source.</span></span> <span data-ttu-id="08fd4-152">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="08fd4-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="08fd4-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="08fd4-153">isDeleted</span></span>|<span data-ttu-id="08fd4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="08fd4-154">Boolean</span></span>|<span data-ttu-id="08fd4-155">指示设备是否从 Apple Business Manager 中删除</span><span class="sxs-lookup"><span data-stu-id="08fd4-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="08fd4-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08fd4-156">createdDateTime</span></span>|<span data-ttu-id="08fd4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fd4-157">DateTimeOffset</span></span>|<span data-ttu-id="08fd4-158">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="08fd4-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="08fd4-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="08fd4-159">lastContactedDateTime</span></span>|<span data-ttu-id="08fd4-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fd4-160">DateTimeOffset</span></span>|<span data-ttu-id="08fd4-161">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="08fd4-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="08fd4-162">说明</span><span class="sxs-lookup"><span data-stu-id="08fd4-162">description</span></span>|<span data-ttu-id="08fd4-163">String</span><span class="sxs-lookup"><span data-stu-id="08fd4-163">String</span></span>|<span data-ttu-id="08fd4-164">设备说明</span><span class="sxs-lookup"><span data-stu-id="08fd4-164">The description of the device</span></span>|
|<span data-ttu-id="08fd4-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="08fd4-165">enrollmentState</span></span>|[<span data-ttu-id="08fd4-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="08fd4-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="08fd4-167">Intune 中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="08fd4-167">The state of the device in Intune.</span></span> <span data-ttu-id="08fd4-168">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="08fd4-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="08fd4-169">平台</span><span class="sxs-lookup"><span data-stu-id="08fd4-169">platform</span></span>|[<span data-ttu-id="08fd4-170">平台</span><span class="sxs-lookup"><span data-stu-id="08fd4-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="08fd4-171">设备平台。</span><span class="sxs-lookup"><span data-stu-id="08fd4-171">The platform of the Device.</span></span> <span data-ttu-id="08fd4-172">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="08fd4-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="08fd4-173">响应</span><span class="sxs-lookup"><span data-stu-id="08fd4-173">Response</span></span>
<span data-ttu-id="08fd4-174">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08fd4-174">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fd4-175">示例</span><span class="sxs-lookup"><span data-stu-id="08fd4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="08fd4-176">请求</span><span class="sxs-lookup"><span data-stu-id="08fd4-176">Request</span></span>
<span data-ttu-id="08fd4-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08fd4-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08fd4-178">响应</span><span class="sxs-lookup"><span data-stu-id="08fd4-178">Response</span></span>
<span data-ttu-id="08fd4-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08fd4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





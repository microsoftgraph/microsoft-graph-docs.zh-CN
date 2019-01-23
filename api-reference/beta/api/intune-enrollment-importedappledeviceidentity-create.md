---
title: 创建 importedAppleDeviceIdentity
description: 创建新的 importedAppleDeviceIdentity 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 839e604fc52c22ff08a963d5601b987780ee241c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422374"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="7ed4a-103">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7ed4a-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="7ed4a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ed4a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ed4a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed4a-107">创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed4a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ed4a-108">Prerequisites</span></span>
<span data-ttu-id="7ed4a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ed4a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ed4a-111">Permission type</span></span>|<span data-ttu-id="7ed4a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ed4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed4a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ed4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed4a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed4a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed4a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ed4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed4a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-116">Not supported.</span></span>|
|<span data-ttu-id="7ed4a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ed4a-117">Application</span></span>|<span data-ttu-id="7ed4a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed4a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ed4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7ed4a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ed4a-120">Request headers</span></span>
|<span data-ttu-id="7ed4a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ed4a-121">Header</span></span>|<span data-ttu-id="7ed4a-122">值</span><span class="sxs-lookup"><span data-stu-id="7ed4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed4a-123">授权</span><span class="sxs-lookup"><span data-stu-id="7ed4a-123">Authorization</span></span>|<span data-ttu-id="7ed4a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ed4a-125">Accept</span></span>|<span data-ttu-id="7ed4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed4a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ed4a-127">Request body</span></span>
<span data-ttu-id="7ed4a-128">在请求正文中，提供 importedAppleDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="7ed4a-129">下表显示时创建 importedAppleDeviceIdentity 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="7ed4a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ed4a-130">Property</span></span>|<span data-ttu-id="7ed4a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ed4a-131">Type</span></span>|<span data-ttu-id="7ed4a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ed4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed4a-133">id</span><span class="sxs-lookup"><span data-stu-id="7ed4a-133">id</span></span>|<span data-ttu-id="7ed4a-134">String</span><span class="sxs-lookup"><span data-stu-id="7ed4a-134">String</span></span>|<span data-ttu-id="7ed4a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-135">Key of the entity.</span></span>|
|<span data-ttu-id="7ed4a-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7ed4a-136">serialNumber</span></span>|<span data-ttu-id="7ed4a-137">String</span><span class="sxs-lookup"><span data-stu-id="7ed4a-137">String</span></span>|<span data-ttu-id="7ed4a-138">设备序列号</span><span class="sxs-lookup"><span data-stu-id="7ed4a-138">Device serial number</span></span>|
|<span data-ttu-id="7ed4a-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="7ed4a-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="7ed4a-140">String</span><span class="sxs-lookup"><span data-stu-id="7ed4a-140">String</span></span>|<span data-ttu-id="7ed4a-141">注册配置文件 Id 管理打算在下一步注册过程适用于设备</span><span class="sxs-lookup"><span data-stu-id="7ed4a-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="7ed4a-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4a-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="7ed4a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4a-143">DateTimeOffset</span></span>|<span data-ttu-id="7ed4a-144">时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="7ed4a-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="7ed4a-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7ed4a-145">isSupervised</span></span>|<span data-ttu-id="7ed4a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed4a-146">Boolean</span></span>|<span data-ttu-id="7ed4a-147">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="7ed4a-148">详细信息位于：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="7ed4a-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="7ed4a-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="7ed4a-149">discoverySource</span></span>|[<span data-ttu-id="7ed4a-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="7ed4a-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="7ed4a-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-151">Apple device discovery source.</span></span> <span data-ttu-id="7ed4a-152">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="7ed4a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4a-153">createdDateTime</span></span>|<span data-ttu-id="7ed4a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4a-154">DateTimeOffset</span></span>|<span data-ttu-id="7ed4a-155">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="7ed4a-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="7ed4a-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4a-156">lastContactedDateTime</span></span>|<span data-ttu-id="7ed4a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4a-157">DateTimeOffset</span></span>|<span data-ttu-id="7ed4a-158">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="7ed4a-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="7ed4a-159">说明</span><span class="sxs-lookup"><span data-stu-id="7ed4a-159">description</span></span>|<span data-ttu-id="7ed4a-160">String</span><span class="sxs-lookup"><span data-stu-id="7ed4a-160">String</span></span>|<span data-ttu-id="7ed4a-161">设备的说明</span><span class="sxs-lookup"><span data-stu-id="7ed4a-161">The description of the device</span></span>|
|<span data-ttu-id="7ed4a-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7ed4a-162">enrollmentState</span></span>|[<span data-ttu-id="7ed4a-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7ed4a-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7ed4a-164">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-164">The state of the device in Intune.</span></span> <span data-ttu-id="7ed4a-165">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7ed4a-166">platform</span><span class="sxs-lookup"><span data-stu-id="7ed4a-166">platform</span></span>|[<span data-ttu-id="7ed4a-167">平台</span><span class="sxs-lookup"><span data-stu-id="7ed4a-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7ed4a-168">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-168">The platform of the Device.</span></span> <span data-ttu-id="7ed4a-169">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ed4a-170">响应</span><span class="sxs-lookup"><span data-stu-id="7ed4a-170">Response</span></span>
<span data-ttu-id="7ed4a-171">如果成功，此方法返回`201 Created`响应代码和响应正文中的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed4a-172">示例</span><span class="sxs-lookup"><span data-stu-id="7ed4a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed4a-173">请求</span><span class="sxs-lookup"><span data-stu-id="7ed4a-173">Request</span></span>
<span data-ttu-id="7ed4a-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="7ed4a-175">响应</span><span class="sxs-lookup"><span data-stu-id="7ed4a-175">Response</span></span>
<span data-ttu-id="7ed4a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ed4a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





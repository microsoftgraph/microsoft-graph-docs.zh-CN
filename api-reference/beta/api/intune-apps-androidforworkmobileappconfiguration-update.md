---
title: 更新 androidForWorkMobileAppConfiguration
description: 更新 androidForWorkMobileAppConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64b208535ac03ffcc3f8b63425efabe896def3df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395263"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="d70a6-103">更新 androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d70a6-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="d70a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d70a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70a6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d70a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70a6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d70a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70a6-107">更新[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d70a6-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d70a6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d70a6-108">Prerequisites</span></span>
<span data-ttu-id="d70a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d70a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70a6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d70a6-111">Permission type</span></span>|<span data-ttu-id="d70a6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d70a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70a6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d70a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d70a6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70a6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d70a6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d70a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d70a6-116">Not supported.</span></span>|
|<span data-ttu-id="d70a6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d70a6-117">Application</span></span>|<span data-ttu-id="d70a6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70a6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70a6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d70a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d70a6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d70a6-120">Request headers</span></span>
|<span data-ttu-id="d70a6-121">标头</span><span class="sxs-lookup"><span data-stu-id="d70a6-121">Header</span></span>|<span data-ttu-id="d70a6-122">值</span><span class="sxs-lookup"><span data-stu-id="d70a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d70a6-123">Authorization</span></span>|<span data-ttu-id="d70a6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d70a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d70a6-125">接受</span><span class="sxs-lookup"><span data-stu-id="d70a6-125">Accept</span></span>|<span data-ttu-id="d70a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d70a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d70a6-127">Request body</span></span>
<span data-ttu-id="d70a6-128">在请求正文中，提供[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d70a6-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="d70a6-129">下表显示创建[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d70a6-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="d70a6-130">属性</span><span class="sxs-lookup"><span data-stu-id="d70a6-130">Property</span></span>|<span data-ttu-id="d70a6-131">类型</span><span class="sxs-lookup"><span data-stu-id="d70a6-131">Type</span></span>|<span data-ttu-id="d70a6-132">说明</span><span class="sxs-lookup"><span data-stu-id="d70a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70a6-133">id</span><span class="sxs-lookup"><span data-stu-id="d70a6-133">id</span></span>|<span data-ttu-id="d70a6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d70a6-134">String</span></span>|<span data-ttu-id="d70a6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d70a6-135">Key of the entity.</span></span> <span data-ttu-id="d70a6-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d70a6-137">targetedMobileApps</span></span>|<span data-ttu-id="d70a6-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="d70a6-138">String collection</span></span>|<span data-ttu-id="d70a6-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="d70a6-139">the associated app.</span></span> <span data-ttu-id="d70a6-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d70a6-141">roleScopeTagIds</span></span>|<span data-ttu-id="d70a6-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d70a6-142">String collection</span></span>|<span data-ttu-id="d70a6-143">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d70a6-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="d70a6-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d70a6-145">createdDateTime</span></span>|<span data-ttu-id="d70a6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d70a6-146">DateTimeOffset</span></span>|<span data-ttu-id="d70a6-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d70a6-147">DateTime the object was created.</span></span> <span data-ttu-id="d70a6-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-149">description</span><span class="sxs-lookup"><span data-stu-id="d70a6-149">description</span></span>|<span data-ttu-id="d70a6-150">String</span><span class="sxs-lookup"><span data-stu-id="d70a6-150">String</span></span>|<span data-ttu-id="d70a6-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="d70a6-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d70a6-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d70a6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d70a6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d70a6-154">DateTimeOffset</span></span>|<span data-ttu-id="d70a6-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d70a6-155">DateTime the object was last modified.</span></span> <span data-ttu-id="d70a6-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-157">displayName</span><span class="sxs-lookup"><span data-stu-id="d70a6-157">displayName</span></span>|<span data-ttu-id="d70a6-158">String</span><span class="sxs-lookup"><span data-stu-id="d70a6-158">String</span></span>|<span data-ttu-id="d70a6-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="d70a6-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d70a6-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-161">version</span><span class="sxs-lookup"><span data-stu-id="d70a6-161">version</span></span>|<span data-ttu-id="d70a6-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d70a6-162">Int32</span></span>|<span data-ttu-id="d70a6-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d70a6-163">Version of the device configuration.</span></span> <span data-ttu-id="d70a6-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d70a6-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d70a6-165">packageId</span><span class="sxs-lookup"><span data-stu-id="d70a6-165">packageId</span></span>|<span data-ttu-id="d70a6-166">String</span><span class="sxs-lookup"><span data-stu-id="d70a6-166">String</span></span>|<span data-ttu-id="d70a6-167">适用于工作的应用程序配置包 id 的 Android。</span><span class="sxs-lookup"><span data-stu-id="d70a6-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="d70a6-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="d70a6-168">payloadJson</span></span>|<span data-ttu-id="d70a6-169">字符串</span><span class="sxs-lookup"><span data-stu-id="d70a6-169">String</span></span>|<span data-ttu-id="d70a6-170">适用于工作的应用程序配置 JSON 负载的 Android。</span><span class="sxs-lookup"><span data-stu-id="d70a6-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="d70a6-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="d70a6-171">permissionActions</span></span>|<span data-ttu-id="d70a6-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="d70a6-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="d70a6-173">Android 应用程序权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="d70a6-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="d70a6-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="d70a6-174">profileApplicability</span></span>|[<span data-ttu-id="d70a6-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="d70a6-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="d70a6-176">Android 企业配置文件适用性（AndroidWorkProfile、DeviceOwner 或 default （适用于两者））。</span><span class="sxs-lookup"><span data-stu-id="d70a6-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="d70a6-177">可取值为：`default`、`androidWorkProfile`、`androidDeviceOwner`。</span><span class="sxs-lookup"><span data-stu-id="d70a6-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="d70a6-178">响应</span><span class="sxs-lookup"><span data-stu-id="d70a6-178">Response</span></span>
<span data-ttu-id="d70a6-179">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d70a6-179">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70a6-180">示例</span><span class="sxs-lookup"><span data-stu-id="d70a6-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="d70a6-181">请求</span><span class="sxs-lookup"><span data-stu-id="d70a6-181">Request</span></span>
<span data-ttu-id="d70a6-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d70a6-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 609

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="d70a6-183">响应</span><span class="sxs-lookup"><span data-stu-id="d70a6-183">Response</span></span>
<span data-ttu-id="d70a6-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d70a6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "profileApplicability": "androidWorkProfile"
}
```




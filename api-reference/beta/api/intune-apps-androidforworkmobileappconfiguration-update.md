---
title: 更新 androidForWorkMobileAppConfiguration
description: 更新 androidForWorkMobileAppConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b37272bc0b7b55a3476bf9dee059380298512644
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445958"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="e6fd0-103">更新 androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6fd0-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="e6fd0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e6fd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6fd0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6fd0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6fd0-107">更新[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6fd0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6fd0-108">Prerequisites</span></span>
<span data-ttu-id="e6fd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6fd0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6fd0-111">Permission type</span></span>|<span data-ttu-id="e6fd0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6fd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6fd0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6fd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6fd0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6fd0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6fd0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6fd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6fd0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-116">Not supported.</span></span>|
|<span data-ttu-id="e6fd0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6fd0-117">Application</span></span>|<span data-ttu-id="e6fd0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6fd0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6fd0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6fd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e6fd0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6fd0-120">Request headers</span></span>
|<span data-ttu-id="e6fd0-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6fd0-121">Header</span></span>|<span data-ttu-id="e6fd0-122">值</span><span class="sxs-lookup"><span data-stu-id="e6fd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6fd0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6fd0-123">Authorization</span></span>|<span data-ttu-id="e6fd0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6fd0-125">接受</span><span class="sxs-lookup"><span data-stu-id="e6fd0-125">Accept</span></span>|<span data-ttu-id="e6fd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6fd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6fd0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6fd0-127">Request body</span></span>
<span data-ttu-id="e6fd0-128">在请求正文中，提供[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="e6fd0-129">下表显示创建[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="e6fd0-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6fd0-130">Property</span></span>|<span data-ttu-id="e6fd0-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6fd0-131">Type</span></span>|<span data-ttu-id="e6fd0-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6fd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6fd0-133">id</span><span class="sxs-lookup"><span data-stu-id="e6fd0-133">id</span></span>|<span data-ttu-id="e6fd0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e6fd0-134">String</span></span>|<span data-ttu-id="e6fd0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-135">Key of the entity.</span></span> <span data-ttu-id="e6fd0-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="e6fd0-137">targetedMobileApps</span></span>|<span data-ttu-id="e6fd0-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6fd0-138">String collection</span></span>|<span data-ttu-id="e6fd0-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-139">the associated app.</span></span> <span data-ttu-id="e6fd0-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6fd0-141">roleScopeTagIds</span></span>|<span data-ttu-id="e6fd0-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6fd0-142">String collection</span></span>|<span data-ttu-id="e6fd0-143">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="e6fd0-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6fd0-145">createdDateTime</span></span>|<span data-ttu-id="e6fd0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6fd0-146">DateTimeOffset</span></span>|<span data-ttu-id="e6fd0-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-147">DateTime the object was created.</span></span> <span data-ttu-id="e6fd0-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-149">说明</span><span class="sxs-lookup"><span data-stu-id="e6fd0-149">description</span></span>|<span data-ttu-id="e6fd0-150">String</span><span class="sxs-lookup"><span data-stu-id="e6fd0-150">String</span></span>|<span data-ttu-id="e6fd0-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6fd0-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6fd0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e6fd0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6fd0-154">DateTimeOffset</span></span>|<span data-ttu-id="e6fd0-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-155">DateTime the object was last modified.</span></span> <span data-ttu-id="e6fd0-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-157">displayName</span><span class="sxs-lookup"><span data-stu-id="e6fd0-157">displayName</span></span>|<span data-ttu-id="e6fd0-158">String</span><span class="sxs-lookup"><span data-stu-id="e6fd0-158">String</span></span>|<span data-ttu-id="e6fd0-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6fd0-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-161">version</span><span class="sxs-lookup"><span data-stu-id="e6fd0-161">version</span></span>|<span data-ttu-id="e6fd0-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e6fd0-162">Int32</span></span>|<span data-ttu-id="e6fd0-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-163">Version of the device configuration.</span></span> <span data-ttu-id="e6fd0-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6fd0-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="e6fd0-165">packageId</span><span class="sxs-lookup"><span data-stu-id="e6fd0-165">packageId</span></span>|<span data-ttu-id="e6fd0-166">String</span><span class="sxs-lookup"><span data-stu-id="e6fd0-166">String</span></span>|<span data-ttu-id="e6fd0-167">适用于工作的应用程序配置包 id 的 Android。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="e6fd0-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="e6fd0-168">payloadJson</span></span>|<span data-ttu-id="e6fd0-169">String</span><span class="sxs-lookup"><span data-stu-id="e6fd0-169">String</span></span>|<span data-ttu-id="e6fd0-170">适用于工作的应用程序配置 JSON 负载的 Android。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="e6fd0-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="e6fd0-171">permissionActions</span></span>|<span data-ttu-id="e6fd0-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6fd0-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="e6fd0-173">Android 应用程序权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="e6fd0-174">响应</span><span class="sxs-lookup"><span data-stu-id="e6fd0-174">Response</span></span>
<span data-ttu-id="e6fd0-175">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6fd0-176">示例</span><span class="sxs-lookup"><span data-stu-id="e6fd0-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6fd0-177">请求</span><span class="sxs-lookup"><span data-stu-id="e6fd0-177">Request</span></span>
<span data-ttu-id="e6fd0-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 560

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="e6fd0-179">响应</span><span class="sxs-lookup"><span data-stu-id="e6fd0-179">Response</span></span>
<span data-ttu-id="e6fd0-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6fd0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 732

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
  ]
}
```






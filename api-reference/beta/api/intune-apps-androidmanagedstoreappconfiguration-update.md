---
title: 更新 androidManagedStoreAppConfiguration
description: 更新 androidManagedStoreAppConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa85985d659d30aa30f4e2f22e2551deeb2fee53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952152"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="26063-103">更新 androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="26063-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="26063-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26063-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26063-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26063-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26063-106">更新[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26063-106">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26063-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26063-107">Prerequisites</span></span>
<span data-ttu-id="26063-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26063-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26063-110">Permission type</span></span>|<span data-ttu-id="26063-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26063-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26063-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26063-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26063-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26063-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26063-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26063-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26063-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26063-115">Not supported.</span></span>|
|<span data-ttu-id="26063-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26063-116">Application</span></span>|<span data-ttu-id="26063-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="26063-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26063-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26063-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="26063-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26063-119">Request headers</span></span>
|<span data-ttu-id="26063-120">标头</span><span class="sxs-lookup"><span data-stu-id="26063-120">Header</span></span>|<span data-ttu-id="26063-121">值</span><span class="sxs-lookup"><span data-stu-id="26063-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26063-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26063-122">Authorization</span></span>|<span data-ttu-id="26063-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26063-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26063-124">接受</span><span class="sxs-lookup"><span data-stu-id="26063-124">Accept</span></span>|<span data-ttu-id="26063-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26063-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26063-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26063-126">Request body</span></span>
<span data-ttu-id="26063-127">在请求正文中, 提供[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26063-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="26063-128">下表显示创建[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="26063-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="26063-129">属性</span><span class="sxs-lookup"><span data-stu-id="26063-129">Property</span></span>|<span data-ttu-id="26063-130">类型</span><span class="sxs-lookup"><span data-stu-id="26063-130">Type</span></span>|<span data-ttu-id="26063-131">说明</span><span class="sxs-lookup"><span data-stu-id="26063-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26063-132">id</span><span class="sxs-lookup"><span data-stu-id="26063-132">id</span></span>|<span data-ttu-id="26063-133">字符串</span><span class="sxs-lookup"><span data-stu-id="26063-133">String</span></span>|<span data-ttu-id="26063-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="26063-134">Key of the entity.</span></span> <span data-ttu-id="26063-135">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="26063-136">targetedMobileApps</span></span>|<span data-ttu-id="26063-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="26063-137">String collection</span></span>|<span data-ttu-id="26063-138">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="26063-138">the associated app.</span></span> <span data-ttu-id="26063-139">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26063-140">roleScopeTagIds</span></span>|<span data-ttu-id="26063-141">String collection</span><span class="sxs-lookup"><span data-stu-id="26063-141">String collection</span></span>|<span data-ttu-id="26063-142">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="26063-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="26063-143">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26063-144">createdDateTime</span></span>|<span data-ttu-id="26063-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26063-145">DateTimeOffset</span></span>|<span data-ttu-id="26063-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="26063-146">DateTime the object was created.</span></span> <span data-ttu-id="26063-147">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-148">说明</span><span class="sxs-lookup"><span data-stu-id="26063-148">description</span></span>|<span data-ttu-id="26063-149">String</span><span class="sxs-lookup"><span data-stu-id="26063-149">String</span></span>|<span data-ttu-id="26063-150">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="26063-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26063-151">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26063-152">lastModifiedDateTime</span></span>|<span data-ttu-id="26063-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26063-153">DateTimeOffset</span></span>|<span data-ttu-id="26063-154">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="26063-154">DateTime the object was last modified.</span></span> <span data-ttu-id="26063-155">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-156">displayName</span><span class="sxs-lookup"><span data-stu-id="26063-156">displayName</span></span>|<span data-ttu-id="26063-157">String</span><span class="sxs-lookup"><span data-stu-id="26063-157">String</span></span>|<span data-ttu-id="26063-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="26063-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26063-159">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-160">version</span><span class="sxs-lookup"><span data-stu-id="26063-160">version</span></span>|<span data-ttu-id="26063-161">Int32</span><span class="sxs-lookup"><span data-stu-id="26063-161">Int32</span></span>|<span data-ttu-id="26063-162">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="26063-162">Version of the device configuration.</span></span> <span data-ttu-id="26063-163">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26063-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="26063-164">packageId</span><span class="sxs-lookup"><span data-stu-id="26063-164">packageId</span></span>|<span data-ttu-id="26063-165">String</span><span class="sxs-lookup"><span data-stu-id="26063-165">String</span></span>|<span data-ttu-id="26063-166">Android 企业应用程序配置包 id。</span><span class="sxs-lookup"><span data-stu-id="26063-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="26063-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="26063-167">payloadJson</span></span>|<span data-ttu-id="26063-168">String</span><span class="sxs-lookup"><span data-stu-id="26063-168">String</span></span>|<span data-ttu-id="26063-169">Android 企业应用配置 JSON 有效负载。</span><span class="sxs-lookup"><span data-stu-id="26063-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="26063-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="26063-170">permissionActions</span></span>|<span data-ttu-id="26063-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="26063-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="26063-172">Android 应用程序权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="26063-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="26063-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="26063-173">appSupportsOemConfig</span></span>|<span data-ttu-id="26063-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="26063-174">Boolean</span></span>|<span data-ttu-id="26063-175">此 AppConfig 是否为 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="26063-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="26063-176">响应</span><span class="sxs-lookup"><span data-stu-id="26063-176">Response</span></span>
<span data-ttu-id="26063-177">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26063-177">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26063-178">示例</span><span class="sxs-lookup"><span data-stu-id="26063-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="26063-179">请求</span><span class="sxs-lookup"><span data-stu-id="26063-179">Request</span></span>
<span data-ttu-id="26063-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26063-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 592

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="26063-181">响应</span><span class="sxs-lookup"><span data-stu-id="26063-181">Response</span></span>
<span data-ttu-id="26063-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26063-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
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
  "appSupportsOemConfig": true
}
```






---
title: 创建 androidManagedStoreAppConfiguration
description: 创建新的 androidManagedStoreAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac28b6d1e02edb9e1513bda9ccc616126eb13cca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140971"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="b4c15-103">创建 androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4c15-103">Create androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="b4c15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4c15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4c15-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4c15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4c15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4c15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c15-107">创建新的 [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4c15-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4c15-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4c15-108">Prerequisites</span></span>
<span data-ttu-id="b4c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4c15-111">Permission type</span></span>|<span data-ttu-id="b4c15-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4c15-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4c15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4c15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4c15-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4c15-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4c15-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4c15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4c15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4c15-116">Not supported.</span></span>|
|<span data-ttu-id="b4c15-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4c15-117">Application</span></span>|<span data-ttu-id="b4c15-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4c15-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4c15-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4c15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4c15-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4c15-120">Request headers</span></span>
|<span data-ttu-id="b4c15-121">标头</span><span class="sxs-lookup"><span data-stu-id="b4c15-121">Header</span></span>|<span data-ttu-id="b4c15-122">值</span><span class="sxs-lookup"><span data-stu-id="b4c15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4c15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4c15-123">Authorization</span></span>|<span data-ttu-id="b4c15-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4c15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4c15-125">接受</span><span class="sxs-lookup"><span data-stu-id="b4c15-125">Accept</span></span>|<span data-ttu-id="b4c15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4c15-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4c15-127">Request body</span></span>
<span data-ttu-id="b4c15-128">在请求正文中，提供 androidManagedStoreAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4c15-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="b4c15-129">下表显示创建 androidManagedStoreAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4c15-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="b4c15-130">属性</span><span class="sxs-lookup"><span data-stu-id="b4c15-130">Property</span></span>|<span data-ttu-id="b4c15-131">类型</span><span class="sxs-lookup"><span data-stu-id="b4c15-131">Type</span></span>|<span data-ttu-id="b4c15-132">说明</span><span class="sxs-lookup"><span data-stu-id="b4c15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c15-133">id</span><span class="sxs-lookup"><span data-stu-id="b4c15-133">id</span></span>|<span data-ttu-id="b4c15-134">String</span><span class="sxs-lookup"><span data-stu-id="b4c15-134">String</span></span>|<span data-ttu-id="b4c15-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4c15-135">Key of the entity.</span></span> <span data-ttu-id="b4c15-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b4c15-137">targetedMobileApps</span></span>|<span data-ttu-id="b4c15-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="b4c15-138">String collection</span></span>|<span data-ttu-id="b4c15-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b4c15-139">the associated app.</span></span> <span data-ttu-id="b4c15-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4c15-141">roleScopeTagIds</span></span>|<span data-ttu-id="b4c15-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b4c15-142">String collection</span></span>|<span data-ttu-id="b4c15-143">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b4c15-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="b4c15-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c15-145">createdDateTime</span></span>|<span data-ttu-id="b4c15-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c15-146">DateTimeOffset</span></span>|<span data-ttu-id="b4c15-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b4c15-147">DateTime the object was created.</span></span> <span data-ttu-id="b4c15-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-149">说明</span><span class="sxs-lookup"><span data-stu-id="b4c15-149">description</span></span>|<span data-ttu-id="b4c15-150">String</span><span class="sxs-lookup"><span data-stu-id="b4c15-150">String</span></span>|<span data-ttu-id="b4c15-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="b4c15-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4c15-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c15-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b4c15-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c15-154">DateTimeOffset</span></span>|<span data-ttu-id="b4c15-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b4c15-155">DateTime the object was last modified.</span></span> <span data-ttu-id="b4c15-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-157">displayName</span><span class="sxs-lookup"><span data-stu-id="b4c15-157">displayName</span></span>|<span data-ttu-id="b4c15-158">String</span><span class="sxs-lookup"><span data-stu-id="b4c15-158">String</span></span>|<span data-ttu-id="b4c15-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="b4c15-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4c15-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-161">version</span><span class="sxs-lookup"><span data-stu-id="b4c15-161">version</span></span>|<span data-ttu-id="b4c15-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c15-162">Int32</span></span>|<span data-ttu-id="b4c15-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b4c15-163">Version of the device configuration.</span></span> <span data-ttu-id="b4c15-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4c15-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4c15-165">packageId</span><span class="sxs-lookup"><span data-stu-id="b4c15-165">packageId</span></span>|<span data-ttu-id="b4c15-166">String</span><span class="sxs-lookup"><span data-stu-id="b4c15-166">String</span></span>|<span data-ttu-id="b4c15-167">Android 企业应用配置包 ID。</span><span class="sxs-lookup"><span data-stu-id="b4c15-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="b4c15-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="b4c15-168">payloadJson</span></span>|<span data-ttu-id="b4c15-169">String</span><span class="sxs-lookup"><span data-stu-id="b4c15-169">String</span></span>|<span data-ttu-id="b4c15-170">Android 企业应用配置 JSON 有效负载。</span><span class="sxs-lookup"><span data-stu-id="b4c15-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="b4c15-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="b4c15-171">permissionActions</span></span>|<span data-ttu-id="b4c15-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4c15-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="b4c15-173">Android 应用权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="b4c15-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="b4c15-174">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="b4c15-174">appSupportsOemConfig</span></span>|<span data-ttu-id="b4c15-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4c15-175">Boolean</span></span>|<span data-ttu-id="b4c15-176">此 AppConfig 是否是 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="b4c15-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|
|<span data-ttu-id="b4c15-177">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="b4c15-177">profileApplicability</span></span>|[<span data-ttu-id="b4c15-178">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="b4c15-178">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="b4c15-179">Android Enterprise 配置文件适用性 (AndroidWorkProfile、DeviceOwner 或默认 (适用于这两) ) 。</span><span class="sxs-lookup"><span data-stu-id="b4c15-179">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="b4c15-180">可取值为：`default`、`androidWorkProfile`、`androidDeviceOwner`。</span><span class="sxs-lookup"><span data-stu-id="b4c15-180">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="b4c15-181">响应</span><span class="sxs-lookup"><span data-stu-id="b4c15-181">Response</span></span>
<span data-ttu-id="b4c15-182">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4c15-182">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c15-183">示例</span><span class="sxs-lookup"><span data-stu-id="b4c15-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4c15-184">请求</span><span class="sxs-lookup"><span data-stu-id="b4c15-184">Request</span></span>
<span data-ttu-id="b4c15-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4c15-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 641

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
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="b4c15-186">响应</span><span class="sxs-lookup"><span data-stu-id="b4c15-186">Response</span></span>
<span data-ttu-id="b4c15-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4c15-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

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
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```





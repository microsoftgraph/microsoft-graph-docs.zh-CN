---
title: 创建 androidManagedStoreAppConfiguration
description: 创建新的 androidManagedStoreAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f55c5e107e4ecdf65f06bcf4a15a42af0facc391
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445888"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="01bc1-103">创建 androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="01bc1-103">Create androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="01bc1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="01bc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01bc1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01bc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01bc1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01bc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01bc1-107">创建新的[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01bc1-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01bc1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="01bc1-108">Prerequisites</span></span>
<span data-ttu-id="01bc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01bc1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="01bc1-111">Permission type</span></span>|<span data-ttu-id="01bc1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="01bc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01bc1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01bc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01bc1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01bc1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01bc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01bc1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="01bc1-116">Not supported.</span></span>|
|<span data-ttu-id="01bc1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="01bc1-117">Application</span></span>|<span data-ttu-id="01bc1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01bc1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01bc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01bc1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="01bc1-120">Request headers</span></span>
|<span data-ttu-id="01bc1-121">标头</span><span class="sxs-lookup"><span data-stu-id="01bc1-121">Header</span></span>|<span data-ttu-id="01bc1-122">值</span><span class="sxs-lookup"><span data-stu-id="01bc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01bc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01bc1-123">Authorization</span></span>|<span data-ttu-id="01bc1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01bc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01bc1-125">接受</span><span class="sxs-lookup"><span data-stu-id="01bc1-125">Accept</span></span>|<span data-ttu-id="01bc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01bc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01bc1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01bc1-127">Request body</span></span>
<span data-ttu-id="01bc1-128">在请求正文中，提供 androidManagedStoreAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01bc1-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="01bc1-129">下表显示创建 androidManagedStoreAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="01bc1-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="01bc1-130">属性</span><span class="sxs-lookup"><span data-stu-id="01bc1-130">Property</span></span>|<span data-ttu-id="01bc1-131">类型</span><span class="sxs-lookup"><span data-stu-id="01bc1-131">Type</span></span>|<span data-ttu-id="01bc1-132">说明</span><span class="sxs-lookup"><span data-stu-id="01bc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01bc1-133">id</span><span class="sxs-lookup"><span data-stu-id="01bc1-133">id</span></span>|<span data-ttu-id="01bc1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="01bc1-134">String</span></span>|<span data-ttu-id="01bc1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="01bc1-135">Key of the entity.</span></span> <span data-ttu-id="01bc1-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="01bc1-137">targetedMobileApps</span></span>|<span data-ttu-id="01bc1-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="01bc1-138">String collection</span></span>|<span data-ttu-id="01bc1-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="01bc1-139">the associated app.</span></span> <span data-ttu-id="01bc1-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01bc1-141">roleScopeTagIds</span></span>|<span data-ttu-id="01bc1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="01bc1-142">String collection</span></span>|<span data-ttu-id="01bc1-143">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="01bc1-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="01bc1-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01bc1-145">createdDateTime</span></span>|<span data-ttu-id="01bc1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01bc1-146">DateTimeOffset</span></span>|<span data-ttu-id="01bc1-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01bc1-147">DateTime the object was created.</span></span> <span data-ttu-id="01bc1-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-149">说明</span><span class="sxs-lookup"><span data-stu-id="01bc1-149">description</span></span>|<span data-ttu-id="01bc1-150">String</span><span class="sxs-lookup"><span data-stu-id="01bc1-150">String</span></span>|<span data-ttu-id="01bc1-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="01bc1-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01bc1-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01bc1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="01bc1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01bc1-154">DateTimeOffset</span></span>|<span data-ttu-id="01bc1-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01bc1-155">DateTime the object was last modified.</span></span> <span data-ttu-id="01bc1-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-157">displayName</span><span class="sxs-lookup"><span data-stu-id="01bc1-157">displayName</span></span>|<span data-ttu-id="01bc1-158">String</span><span class="sxs-lookup"><span data-stu-id="01bc1-158">String</span></span>|<span data-ttu-id="01bc1-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="01bc1-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01bc1-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-161">version</span><span class="sxs-lookup"><span data-stu-id="01bc1-161">version</span></span>|<span data-ttu-id="01bc1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="01bc1-162">Int32</span></span>|<span data-ttu-id="01bc1-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="01bc1-163">Version of the device configuration.</span></span> <span data-ttu-id="01bc1-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc1-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="01bc1-165">packageId</span><span class="sxs-lookup"><span data-stu-id="01bc1-165">packageId</span></span>|<span data-ttu-id="01bc1-166">String</span><span class="sxs-lookup"><span data-stu-id="01bc1-166">String</span></span>|<span data-ttu-id="01bc1-167">Android 企业应用程序配置包 id。</span><span class="sxs-lookup"><span data-stu-id="01bc1-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="01bc1-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="01bc1-168">payloadJson</span></span>|<span data-ttu-id="01bc1-169">String</span><span class="sxs-lookup"><span data-stu-id="01bc1-169">String</span></span>|<span data-ttu-id="01bc1-170">Android 企业应用配置 JSON 有效负载。</span><span class="sxs-lookup"><span data-stu-id="01bc1-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="01bc1-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="01bc1-171">permissionActions</span></span>|<span data-ttu-id="01bc1-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="01bc1-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="01bc1-173">Android 应用程序权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="01bc1-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="01bc1-174">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="01bc1-174">appSupportsOemConfig</span></span>|<span data-ttu-id="01bc1-175">布尔</span><span class="sxs-lookup"><span data-stu-id="01bc1-175">Boolean</span></span>|<span data-ttu-id="01bc1-176">此 AppConfig 是否为 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="01bc1-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="01bc1-177">响应</span><span class="sxs-lookup"><span data-stu-id="01bc1-177">Response</span></span>
<span data-ttu-id="01bc1-178">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01bc1-178">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01bc1-179">示例</span><span class="sxs-lookup"><span data-stu-id="01bc1-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="01bc1-180">请求</span><span class="sxs-lookup"><span data-stu-id="01bc1-180">Request</span></span>
<span data-ttu-id="01bc1-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01bc1-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="01bc1-182">响应</span><span class="sxs-lookup"><span data-stu-id="01bc1-182">Response</span></span>
<span data-ttu-id="01bc1-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01bc1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






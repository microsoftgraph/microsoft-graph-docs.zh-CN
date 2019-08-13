---
title: 创建 androidForWorkMobileAppConfiguration
description: 创建新的 androidForWorkMobileAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a19ce32f8659e968a3eee0bb99073278b7ed792
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324880"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="4340f-103">创建 androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4340f-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="4340f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4340f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4340f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4340f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4340f-106">创建新的[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4340f-106">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4340f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4340f-107">Prerequisites</span></span>
<span data-ttu-id="4340f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4340f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4340f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4340f-110">Permission type</span></span>|<span data-ttu-id="4340f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4340f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4340f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4340f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4340f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4340f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4340f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4340f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4340f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4340f-115">Not supported.</span></span>|
|<span data-ttu-id="4340f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4340f-116">Application</span></span>|<span data-ttu-id="4340f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4340f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4340f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4340f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4340f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4340f-119">Request headers</span></span>
|<span data-ttu-id="4340f-120">标头</span><span class="sxs-lookup"><span data-stu-id="4340f-120">Header</span></span>|<span data-ttu-id="4340f-121">值</span><span class="sxs-lookup"><span data-stu-id="4340f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4340f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4340f-122">Authorization</span></span>|<span data-ttu-id="4340f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4340f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4340f-124">接受</span><span class="sxs-lookup"><span data-stu-id="4340f-124">Accept</span></span>|<span data-ttu-id="4340f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4340f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4340f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4340f-126">Request body</span></span>
<span data-ttu-id="4340f-127">在请求正文中, 提供 androidForWorkMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4340f-127">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="4340f-128">下表显示创建 androidForWorkMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4340f-128">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="4340f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4340f-129">Property</span></span>|<span data-ttu-id="4340f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4340f-130">Type</span></span>|<span data-ttu-id="4340f-131">说明</span><span class="sxs-lookup"><span data-stu-id="4340f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4340f-132">id</span><span class="sxs-lookup"><span data-stu-id="4340f-132">id</span></span>|<span data-ttu-id="4340f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4340f-133">String</span></span>|<span data-ttu-id="4340f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4340f-134">Key of the entity.</span></span> <span data-ttu-id="4340f-135">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4340f-136">targetedMobileApps</span></span>|<span data-ttu-id="4340f-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="4340f-137">String collection</span></span>|<span data-ttu-id="4340f-138">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="4340f-138">the associated app.</span></span> <span data-ttu-id="4340f-139">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4340f-140">roleScopeTagIds</span></span>|<span data-ttu-id="4340f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4340f-141">String collection</span></span>|<span data-ttu-id="4340f-142">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4340f-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="4340f-143">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4340f-144">createdDateTime</span></span>|<span data-ttu-id="4340f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4340f-145">DateTimeOffset</span></span>|<span data-ttu-id="4340f-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4340f-146">DateTime the object was created.</span></span> <span data-ttu-id="4340f-147">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-148">说明</span><span class="sxs-lookup"><span data-stu-id="4340f-148">description</span></span>|<span data-ttu-id="4340f-149">String</span><span class="sxs-lookup"><span data-stu-id="4340f-149">String</span></span>|<span data-ttu-id="4340f-150">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="4340f-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4340f-151">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4340f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="4340f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4340f-153">DateTimeOffset</span></span>|<span data-ttu-id="4340f-154">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4340f-154">DateTime the object was last modified.</span></span> <span data-ttu-id="4340f-155">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="4340f-156">displayName</span></span>|<span data-ttu-id="4340f-157">String</span><span class="sxs-lookup"><span data-stu-id="4340f-157">String</span></span>|<span data-ttu-id="4340f-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="4340f-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4340f-159">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-160">version</span><span class="sxs-lookup"><span data-stu-id="4340f-160">version</span></span>|<span data-ttu-id="4340f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4340f-161">Int32</span></span>|<span data-ttu-id="4340f-162">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4340f-162">Version of the device configuration.</span></span> <span data-ttu-id="4340f-163">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4340f-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4340f-164">packageId</span><span class="sxs-lookup"><span data-stu-id="4340f-164">packageId</span></span>|<span data-ttu-id="4340f-165">String</span><span class="sxs-lookup"><span data-stu-id="4340f-165">String</span></span>|<span data-ttu-id="4340f-166">适用于工作的应用程序配置包 id 的 Android。</span><span class="sxs-lookup"><span data-stu-id="4340f-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="4340f-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="4340f-167">payloadJson</span></span>|<span data-ttu-id="4340f-168">String</span><span class="sxs-lookup"><span data-stu-id="4340f-168">String</span></span>|<span data-ttu-id="4340f-169">适用于工作的应用程序配置 JSON 负载的 Android。</span><span class="sxs-lookup"><span data-stu-id="4340f-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="4340f-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="4340f-170">permissionActions</span></span>|<span data-ttu-id="4340f-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="4340f-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="4340f-172">Android 应用程序权限和相应权限操作的列表。</span><span class="sxs-lookup"><span data-stu-id="4340f-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="4340f-173">响应</span><span class="sxs-lookup"><span data-stu-id="4340f-173">Response</span></span>
<span data-ttu-id="4340f-174">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4340f-174">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4340f-175">示例</span><span class="sxs-lookup"><span data-stu-id="4340f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4340f-176">请求</span><span class="sxs-lookup"><span data-stu-id="4340f-176">Request</span></span>
<span data-ttu-id="4340f-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4340f-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="4340f-178">响应</span><span class="sxs-lookup"><span data-stu-id="4340f-178">Response</span></span>
<span data-ttu-id="4340f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4340f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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







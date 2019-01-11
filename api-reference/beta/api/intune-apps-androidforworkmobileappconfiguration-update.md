---
title: 更新 androidForWorkMobileAppConfiguration
description: 更新 androidForWorkMobileAppConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e7e593a146b075900e7ce3a59ce5bf49a9f05c02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838099"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="d5c8f-103">更新 androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5c8f-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="d5c8f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5c8f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c8f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5c8f-107">更新[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5c8f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5c8f-108">Prerequisites</span></span>
<span data-ttu-id="d5c8f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d5c8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c8f-111">Permission type</span></span>|<span data-ttu-id="d5c8f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5c8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-116">Not supported.</span></span>|
|<span data-ttu-id="d5c8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5c8f-117">Application</span></span>|<span data-ttu-id="d5c8f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c8f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d5c8f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c8f-120">Request headers</span></span>
|<span data-ttu-id="d5c8f-121">标头</span><span class="sxs-lookup"><span data-stu-id="d5c8f-121">Header</span></span>|<span data-ttu-id="d5c8f-122">值</span><span class="sxs-lookup"><span data-stu-id="d5c8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c8f-123">Authorization</span></span>|<span data-ttu-id="d5c8f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c8f-125">Accept</span></span>|<span data-ttu-id="d5c8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c8f-127">Request body</span></span>
<span data-ttu-id="d5c8f-128">在请求正文中，提供[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="d5c8f-129">下表显示时创建[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="d5c8f-130">属性</span><span class="sxs-lookup"><span data-stu-id="d5c8f-130">Property</span></span>|<span data-ttu-id="d5c8f-131">类型</span><span class="sxs-lookup"><span data-stu-id="d5c8f-131">Type</span></span>|<span data-ttu-id="d5c8f-132">说明</span><span class="sxs-lookup"><span data-stu-id="d5c8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c8f-133">id</span><span class="sxs-lookup"><span data-stu-id="d5c8f-133">id</span></span>|<span data-ttu-id="d5c8f-134">String</span><span class="sxs-lookup"><span data-stu-id="d5c8f-134">String</span></span>|<span data-ttu-id="d5c8f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-135">Key of the entity.</span></span> <span data-ttu-id="d5c8f-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d5c8f-137">targetedMobileApps</span></span>|<span data-ttu-id="d5c8f-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="d5c8f-138">String collection</span></span>|<span data-ttu-id="d5c8f-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-139">the associated app.</span></span> <span data-ttu-id="d5c8f-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5c8f-141">roleScopeTagIds</span></span>|<span data-ttu-id="d5c8f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d5c8f-142">String collection</span></span>|<span data-ttu-id="d5c8f-143">此应用程序配置实体范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="d5c8f-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5c8f-145">createdDateTime</span></span>|<span data-ttu-id="d5c8f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5c8f-146">DateTimeOffset</span></span>|<span data-ttu-id="d5c8f-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-147">DateTime the object was created.</span></span> <span data-ttu-id="d5c8f-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-149">description</span><span class="sxs-lookup"><span data-stu-id="d5c8f-149">description</span></span>|<span data-ttu-id="d5c8f-150">String</span><span class="sxs-lookup"><span data-stu-id="d5c8f-150">String</span></span>|<span data-ttu-id="d5c8f-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5c8f-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5c8f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d5c8f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5c8f-154">DateTimeOffset</span></span>|<span data-ttu-id="d5c8f-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-155">DateTime the object was last modified.</span></span> <span data-ttu-id="d5c8f-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-157">displayName</span><span class="sxs-lookup"><span data-stu-id="d5c8f-157">displayName</span></span>|<span data-ttu-id="d5c8f-158">String</span><span class="sxs-lookup"><span data-stu-id="d5c8f-158">String</span></span>|<span data-ttu-id="d5c8f-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5c8f-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-161">version</span><span class="sxs-lookup"><span data-stu-id="d5c8f-161">version</span></span>|<span data-ttu-id="d5c8f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c8f-162">Int32</span></span>|<span data-ttu-id="d5c8f-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-163">Version of the device configuration.</span></span> <span data-ttu-id="d5c8f-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5c8f-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d5c8f-165">packageId</span><span class="sxs-lookup"><span data-stu-id="d5c8f-165">packageId</span></span>|<span data-ttu-id="d5c8f-166">String</span><span class="sxs-lookup"><span data-stu-id="d5c8f-166">String</span></span>|<span data-ttu-id="d5c8f-167">Android 的工作应用程序配置程序包 id。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="d5c8f-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="d5c8f-168">payloadJson</span></span>|<span data-ttu-id="d5c8f-169">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c8f-169">String</span></span>|<span data-ttu-id="d5c8f-170">为工作 android 应用程序配置 JSON 负载。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="d5c8f-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="d5c8f-171">permissionActions</span></span>|<span data-ttu-id="d5c8f-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="d5c8f-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="d5c8f-173">Android 应用程序权限和权限的相应操作的列表。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="d5c8f-174">响应</span><span class="sxs-lookup"><span data-stu-id="d5c8f-174">Response</span></span>
<span data-ttu-id="d5c8f-175">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c8f-176">示例</span><span class="sxs-lookup"><span data-stu-id="d5c8f-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5c8f-177">请求</span><span class="sxs-lookup"><span data-stu-id="d5c8f-177">Request</span></span>
<span data-ttu-id="d5c8f-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 549

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="d5c8f-179">响应</span><span class="sxs-lookup"><span data-stu-id="d5c8f-179">Response</span></span>
<span data-ttu-id="d5c8f-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5c8f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






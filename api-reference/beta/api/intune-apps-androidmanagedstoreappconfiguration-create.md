---
title: 创建 androidManagedStoreAppConfiguration
description: 创建新的 androidManagedStoreAppConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8768079b14ac0993df63eaa443d078069bb170c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814159"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="20bc4-103">创建 androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="20bc4-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="20bc4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="20bc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20bc4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="20bc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20bc4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20bc4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20bc4-107">创建新的[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20bc4-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20bc4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="20bc4-108">Prerequisites</span></span>
<span data-ttu-id="20bc4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="20bc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20bc4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20bc4-111">Permission type</span></span>|<span data-ttu-id="20bc4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20bc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20bc4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20bc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20bc4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20bc4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20bc4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20bc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20bc4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20bc4-116">Not supported.</span></span>|
|<span data-ttu-id="20bc4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20bc4-117">Application</span></span>|<span data-ttu-id="20bc4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="20bc4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20bc4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20bc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="20bc4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20bc4-120">Request headers</span></span>
|<span data-ttu-id="20bc4-121">标头</span><span class="sxs-lookup"><span data-stu-id="20bc4-121">Header</span></span>|<span data-ttu-id="20bc4-122">值</span><span class="sxs-lookup"><span data-stu-id="20bc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20bc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20bc4-123">Authorization</span></span>|<span data-ttu-id="20bc4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20bc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20bc4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20bc4-125">Accept</span></span>|<span data-ttu-id="20bc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20bc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20bc4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20bc4-127">Request body</span></span>
<span data-ttu-id="20bc4-128">在请求正文中，提供 androidManagedStoreAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20bc4-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="20bc4-129">下表显示时创建 androidManagedStoreAppConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20bc4-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="20bc4-130">属性</span><span class="sxs-lookup"><span data-stu-id="20bc4-130">Property</span></span>|<span data-ttu-id="20bc4-131">类型</span><span class="sxs-lookup"><span data-stu-id="20bc4-131">Type</span></span>|<span data-ttu-id="20bc4-132">说明</span><span class="sxs-lookup"><span data-stu-id="20bc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20bc4-133">id</span><span class="sxs-lookup"><span data-stu-id="20bc4-133">id</span></span>|<span data-ttu-id="20bc4-134">String</span><span class="sxs-lookup"><span data-stu-id="20bc4-134">String</span></span>|<span data-ttu-id="20bc4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="20bc4-135">Key of the entity.</span></span> <span data-ttu-id="20bc4-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="20bc4-137">targetedMobileApps</span></span>|<span data-ttu-id="20bc4-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="20bc4-138">String collection</span></span>|<span data-ttu-id="20bc4-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="20bc4-139">the associated app.</span></span> <span data-ttu-id="20bc4-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20bc4-141">roleScopeTagIds</span></span>|<span data-ttu-id="20bc4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="20bc4-142">String collection</span></span>|<span data-ttu-id="20bc4-143">此应用程序配置实体范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="20bc4-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="20bc4-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20bc4-145">createdDateTime</span></span>|<span data-ttu-id="20bc4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20bc4-146">DateTimeOffset</span></span>|<span data-ttu-id="20bc4-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="20bc4-147">DateTime the object was created.</span></span> <span data-ttu-id="20bc4-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-149">description</span><span class="sxs-lookup"><span data-stu-id="20bc4-149">description</span></span>|<span data-ttu-id="20bc4-150">String</span><span class="sxs-lookup"><span data-stu-id="20bc4-150">String</span></span>|<span data-ttu-id="20bc4-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="20bc4-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20bc4-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20bc4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="20bc4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20bc4-154">DateTimeOffset</span></span>|<span data-ttu-id="20bc4-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="20bc4-155">DateTime the object was last modified.</span></span> <span data-ttu-id="20bc4-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-157">displayName</span><span class="sxs-lookup"><span data-stu-id="20bc4-157">displayName</span></span>|<span data-ttu-id="20bc4-158">String</span><span class="sxs-lookup"><span data-stu-id="20bc4-158">String</span></span>|<span data-ttu-id="20bc4-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="20bc4-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20bc4-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-161">version</span><span class="sxs-lookup"><span data-stu-id="20bc4-161">version</span></span>|<span data-ttu-id="20bc4-162">Int32</span><span class="sxs-lookup"><span data-stu-id="20bc4-162">Int32</span></span>|<span data-ttu-id="20bc4-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="20bc4-163">Version of the device configuration.</span></span> <span data-ttu-id="20bc4-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20bc4-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="20bc4-165">packageId</span><span class="sxs-lookup"><span data-stu-id="20bc4-165">packageId</span></span>|<span data-ttu-id="20bc4-166">String</span><span class="sxs-lookup"><span data-stu-id="20bc4-166">String</span></span>|<span data-ttu-id="20bc4-167">Android 企业应用程序配置程序包 id。</span><span class="sxs-lookup"><span data-stu-id="20bc4-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="20bc4-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="20bc4-168">payloadJson</span></span>|<span data-ttu-id="20bc4-169">字符串</span><span class="sxs-lookup"><span data-stu-id="20bc4-169">String</span></span>|<span data-ttu-id="20bc4-170">Android 企业应用程序配置 JSON 负载。</span><span class="sxs-lookup"><span data-stu-id="20bc4-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="20bc4-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="20bc4-171">permissionActions</span></span>|<span data-ttu-id="20bc4-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="20bc4-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="20bc4-173">Android 应用程序权限和权限的相应操作的列表。</span><span class="sxs-lookup"><span data-stu-id="20bc4-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="20bc4-174">响应</span><span class="sxs-lookup"><span data-stu-id="20bc4-174">Response</span></span>
<span data-ttu-id="20bc4-175">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20bc4-175">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20bc4-176">示例</span><span class="sxs-lookup"><span data-stu-id="20bc4-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="20bc4-177">请求</span><span class="sxs-lookup"><span data-stu-id="20bc4-177">Request</span></span>
<span data-ttu-id="20bc4-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20bc4-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 623

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="20bc4-179">响应</span><span class="sxs-lookup"><span data-stu-id="20bc4-179">Response</span></span>
<span data-ttu-id="20bc4-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20bc4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 731

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
  ]
}
```






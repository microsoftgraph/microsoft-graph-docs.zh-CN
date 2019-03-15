---
title: 创建 androidManagedAppRegistration
description: 创建新的 androidManagedAppRegistration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c05ba7fa13577134b148c8af836e3ba453a1e40
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571457"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="6dc52-103">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6dc52-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="6dc52-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6dc52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc52-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6dc52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc52-106">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6dc52-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc52-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6dc52-107">Prerequisites</span></span>
<span data-ttu-id="6dc52-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6dc52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6dc52-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dc52-110">Permission type</span></span>|<span data-ttu-id="6dc52-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6dc52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc52-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dc52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc52-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc52-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc52-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dc52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc52-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dc52-115">Not supported.</span></span>|
|<span data-ttu-id="6dc52-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dc52-116">Application</span></span>|<span data-ttu-id="6dc52-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dc52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc52-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dc52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="6dc52-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dc52-119">Request headers</span></span>
|<span data-ttu-id="6dc52-120">标头</span><span class="sxs-lookup"><span data-stu-id="6dc52-120">Header</span></span>|<span data-ttu-id="6dc52-121">值</span><span class="sxs-lookup"><span data-stu-id="6dc52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc52-122">Authorization</span></span>|<span data-ttu-id="6dc52-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6dc52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc52-124">接受</span><span class="sxs-lookup"><span data-stu-id="6dc52-124">Accept</span></span>|<span data-ttu-id="6dc52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc52-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dc52-126">Request body</span></span>
<span data-ttu-id="6dc52-127">在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dc52-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="6dc52-128">下表显示了创建 androidManagedAppRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6dc52-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="6dc52-129">属性</span><span class="sxs-lookup"><span data-stu-id="6dc52-129">Property</span></span>|<span data-ttu-id="6dc52-130">类型</span><span class="sxs-lookup"><span data-stu-id="6dc52-130">Type</span></span>|<span data-ttu-id="6dc52-131">说明</span><span class="sxs-lookup"><span data-stu-id="6dc52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc52-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc52-132">createdDateTime</span></span>|<span data-ttu-id="6dc52-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc52-133">DateTimeOffset</span></span>|<span data-ttu-id="6dc52-134">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc52-135">lastSyncDateTime</span></span>|<span data-ttu-id="6dc52-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc52-136">DateTimeOffset</span></span>|<span data-ttu-id="6dc52-137">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6dc52-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="6dc52-138">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6dc52-139">applicationVersion</span></span>|<span data-ttu-id="6dc52-140">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-140">String</span></span>|<span data-ttu-id="6dc52-141">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6dc52-142">managementSdkVersion</span></span>|<span data-ttu-id="6dc52-143">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-143">String</span></span>|<span data-ttu-id="6dc52-144">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6dc52-145">platformVersion</span></span>|<span data-ttu-id="6dc52-146">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-146">String</span></span>|<span data-ttu-id="6dc52-147">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="6dc52-148">deviceType</span></span>|<span data-ttu-id="6dc52-149">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-149">String</span></span>|<span data-ttu-id="6dc52-150">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6dc52-151">deviceTag</span></span>|<span data-ttu-id="6dc52-152">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-152">String</span></span>|<span data-ttu-id="6dc52-153">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="6dc52-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6dc52-154">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="6dc52-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="6dc52-155">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="6dc52-156">deviceName</span></span>|<span data-ttu-id="6dc52-157">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-157">String</span></span>|<span data-ttu-id="6dc52-158">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-159">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6dc52-159">managedDeviceId</span></span>|<span data-ttu-id="6dc52-160">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-160">String</span></span>|<span data-ttu-id="6dc52-161">主机设备的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="6dc52-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="6dc52-162">即使在托管主机设备时, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="6dc52-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="6dc52-163">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="6dc52-164">azureADDeviceId</span></span>|<span data-ttu-id="6dc52-165">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-165">String</span></span>|<span data-ttu-id="6dc52-166">主机设备的 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="6dc52-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="6dc52-167">即使主机设备注册了 Azure Active Directory, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="6dc52-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="6dc52-168">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6dc52-169">deviceModel</span></span>|<span data-ttu-id="6dc52-170">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-170">String</span></span>|<span data-ttu-id="6dc52-171">从[managedAppRegistration](../resources/intune-mam-managedappregistration.md)继承的当前应用注册的设备模型</span><span class="sxs-lookup"><span data-stu-id="6dc52-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-172">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="6dc52-172">deviceManufacturer</span></span>|<span data-ttu-id="6dc52-173">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-173">String</span></span>|<span data-ttu-id="6dc52-174">从[managedAppRegistration](../resources/intune-mam-managedappregistration.md)继承的当前应用注册的设备制造商</span><span class="sxs-lookup"><span data-stu-id="6dc52-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6dc52-175">flaggedReasons</span></span>|<span data-ttu-id="6dc52-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="6dc52-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6dc52-177">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="6dc52-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6dc52-178">例如，</span><span class="sxs-lookup"><span data-stu-id="6dc52-178">E.g.</span></span> <span data-ttu-id="6dc52-179">在从[managedAppRegistration](../resources/intune-mam-managedappregistration.md)继承的根设备上运行的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6dc52-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="6dc52-180">可取值为：`none`、`rootedDevice`、`androidBootloaderUnlocked`、`androidFactoryRomModified`。</span><span class="sxs-lookup"><span data-stu-id="6dc52-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="6dc52-181">userId</span><span class="sxs-lookup"><span data-stu-id="6dc52-181">userId</span></span>|<span data-ttu-id="6dc52-182">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-182">String</span></span>|<span data-ttu-id="6dc52-183">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6dc52-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="6dc52-184">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6dc52-185">appIdentifier</span></span>|[<span data-ttu-id="6dc52-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6dc52-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6dc52-187">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-188">id</span><span class="sxs-lookup"><span data-stu-id="6dc52-188">id</span></span>|<span data-ttu-id="6dc52-189">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-189">String</span></span>|<span data-ttu-id="6dc52-190">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6dc52-190">Key of the entity.</span></span> <span data-ttu-id="6dc52-191">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-192">version</span><span class="sxs-lookup"><span data-stu-id="6dc52-192">version</span></span>|<span data-ttu-id="6dc52-193">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-193">String</span></span>|<span data-ttu-id="6dc52-194">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6dc52-194">Version of the entity.</span></span> <span data-ttu-id="6dc52-195">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc52-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6dc52-196">patchVersion</span><span class="sxs-lookup"><span data-stu-id="6dc52-196">patchVersion</span></span>|<span data-ttu-id="6dc52-197">String</span><span class="sxs-lookup"><span data-stu-id="6dc52-197">String</span></span>|<span data-ttu-id="6dc52-198">当前 android 应用注册的修补程序版本</span><span class="sxs-lookup"><span data-stu-id="6dc52-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="6dc52-199">响应</span><span class="sxs-lookup"><span data-stu-id="6dc52-199">Response</span></span>
<span data-ttu-id="6dc52-200">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6dc52-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc52-201">示例</span><span class="sxs-lookup"><span data-stu-id="6dc52-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc52-202">请求</span><span class="sxs-lookup"><span data-stu-id="6dc52-202">Request</span></span>
<span data-ttu-id="6dc52-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dc52-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="6dc52-204">响应</span><span class="sxs-lookup"><span data-stu-id="6dc52-204">Response</span></span>
<span data-ttu-id="6dc52-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dc52-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```





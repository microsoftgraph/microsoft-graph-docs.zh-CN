---
title: 创建 androidManagedAppRegistration
description: 创建新的 androidManagedAppRegistration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3c0b4901db4ee277b4f2470bc62aaffd00bbea3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145528"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="a727f-103">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a727f-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="a727f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a727f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a727f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a727f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a727f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a727f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a727f-107">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a727f-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a727f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a727f-108">Prerequisites</span></span>
<span data-ttu-id="a727f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a727f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a727f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a727f-111">Permission type</span></span>|<span data-ttu-id="a727f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a727f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a727f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a727f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a727f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a727f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a727f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a727f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a727f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a727f-116">Not supported.</span></span>|
|<span data-ttu-id="a727f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a727f-117">Application</span></span>|<span data-ttu-id="a727f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a727f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a727f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a727f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="a727f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a727f-120">Request headers</span></span>
|<span data-ttu-id="a727f-121">标头</span><span class="sxs-lookup"><span data-stu-id="a727f-121">Header</span></span>|<span data-ttu-id="a727f-122">值</span><span class="sxs-lookup"><span data-stu-id="a727f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a727f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a727f-123">Authorization</span></span>|<span data-ttu-id="a727f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a727f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a727f-125">接受</span><span class="sxs-lookup"><span data-stu-id="a727f-125">Accept</span></span>|<span data-ttu-id="a727f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a727f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a727f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a727f-127">Request body</span></span>
<span data-ttu-id="a727f-128">在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a727f-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="a727f-129">下表显示了创建 androidManagedAppRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a727f-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="a727f-130">属性</span><span class="sxs-lookup"><span data-stu-id="a727f-130">Property</span></span>|<span data-ttu-id="a727f-131">类型</span><span class="sxs-lookup"><span data-stu-id="a727f-131">Type</span></span>|<span data-ttu-id="a727f-132">说明</span><span class="sxs-lookup"><span data-stu-id="a727f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a727f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a727f-133">createdDateTime</span></span>|<span data-ttu-id="a727f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a727f-134">DateTimeOffset</span></span>|<span data-ttu-id="a727f-135">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a727f-136">lastSyncDateTime</span></span>|<span data-ttu-id="a727f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a727f-137">DateTimeOffset</span></span>|<span data-ttu-id="a727f-138">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a727f-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="a727f-139">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="a727f-140">applicationVersion</span></span>|<span data-ttu-id="a727f-141">String</span><span class="sxs-lookup"><span data-stu-id="a727f-141">String</span></span>|<span data-ttu-id="a727f-142">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="a727f-143">managementSdkVersion</span></span>|<span data-ttu-id="a727f-144">String</span><span class="sxs-lookup"><span data-stu-id="a727f-144">String</span></span>|<span data-ttu-id="a727f-145">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="a727f-146">platformVersion</span></span>|<span data-ttu-id="a727f-147">String</span><span class="sxs-lookup"><span data-stu-id="a727f-147">String</span></span>|<span data-ttu-id="a727f-148">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="a727f-149">deviceType</span></span>|<span data-ttu-id="a727f-150">String</span><span class="sxs-lookup"><span data-stu-id="a727f-150">String</span></span>|<span data-ttu-id="a727f-151">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="a727f-152">deviceTag</span></span>|<span data-ttu-id="a727f-153">String</span><span class="sxs-lookup"><span data-stu-id="a727f-153">String</span></span>|<span data-ttu-id="a727f-154">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="a727f-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="a727f-155">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="a727f-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="a727f-156">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="a727f-157">deviceName</span></span>|<span data-ttu-id="a727f-158">String</span><span class="sxs-lookup"><span data-stu-id="a727f-158">String</span></span>|<span data-ttu-id="a727f-159">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a727f-160">managedDeviceId</span></span>|<span data-ttu-id="a727f-161">String</span><span class="sxs-lookup"><span data-stu-id="a727f-161">String</span></span>|<span data-ttu-id="a727f-162">主机设备的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="a727f-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="a727f-163">即使托管主机设备，值也可以为空。</span><span class="sxs-lookup"><span data-stu-id="a727f-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="a727f-164">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a727f-165">azureADDeviceId</span></span>|<span data-ttu-id="a727f-166">String</span><span class="sxs-lookup"><span data-stu-id="a727f-166">String</span></span>|<span data-ttu-id="a727f-167">主机设备的 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="a727f-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="a727f-168">即使主机设备已注册 Azure Active Directory，值也可以为空。</span><span class="sxs-lookup"><span data-stu-id="a727f-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="a727f-169">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a727f-170">deviceModel</span></span>|<span data-ttu-id="a727f-171">String</span><span class="sxs-lookup"><span data-stu-id="a727f-171">String</span></span>|<span data-ttu-id="a727f-172">当前应用注册的设备型号 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="a727f-173">deviceManufacturer</span></span>|<span data-ttu-id="a727f-174">String</span><span class="sxs-lookup"><span data-stu-id="a727f-174">String</span></span>|<span data-ttu-id="a727f-175">当前应用注册的设备制造商 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="a727f-176">flaggedReasons</span></span>|<span data-ttu-id="a727f-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a727f-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="a727f-178">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="a727f-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="a727f-179">例如，</span><span class="sxs-lookup"><span data-stu-id="a727f-179">E.g.</span></span> <span data-ttu-id="a727f-180">在根设备上运行的应用 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)。</span><span class="sxs-lookup"><span data-stu-id="a727f-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="a727f-181">可取值为：`none`、`rootedDevice`、`androidBootloaderUnlocked`、`androidFactoryRomModified`。</span><span class="sxs-lookup"><span data-stu-id="a727f-181">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="a727f-182">userId</span><span class="sxs-lookup"><span data-stu-id="a727f-182">userId</span></span>|<span data-ttu-id="a727f-183">String</span><span class="sxs-lookup"><span data-stu-id="a727f-183">String</span></span>|<span data-ttu-id="a727f-184">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="a727f-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="a727f-185">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a727f-186">appIdentifier</span></span>|[<span data-ttu-id="a727f-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a727f-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a727f-188">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-189">id</span><span class="sxs-lookup"><span data-stu-id="a727f-189">id</span></span>|<span data-ttu-id="a727f-190">String</span><span class="sxs-lookup"><span data-stu-id="a727f-190">String</span></span>|<span data-ttu-id="a727f-191">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a727f-191">Key of the entity.</span></span> <span data-ttu-id="a727f-192">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-193">version</span><span class="sxs-lookup"><span data-stu-id="a727f-193">version</span></span>|<span data-ttu-id="a727f-194">String</span><span class="sxs-lookup"><span data-stu-id="a727f-194">String</span></span>|<span data-ttu-id="a727f-195">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a727f-195">Version of the entity.</span></span> <span data-ttu-id="a727f-196">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a727f-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a727f-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="a727f-197">patchVersion</span></span>|<span data-ttu-id="a727f-198">String</span><span class="sxs-lookup"><span data-stu-id="a727f-198">String</span></span>|<span data-ttu-id="a727f-199">当前 android 应用注册的修补程序版本</span><span class="sxs-lookup"><span data-stu-id="a727f-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="a727f-200">响应</span><span class="sxs-lookup"><span data-stu-id="a727f-200">Response</span></span>
<span data-ttu-id="a727f-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a727f-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a727f-202">示例</span><span class="sxs-lookup"><span data-stu-id="a727f-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="a727f-203">请求</span><span class="sxs-lookup"><span data-stu-id="a727f-203">Request</span></span>
<span data-ttu-id="a727f-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a727f-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a727f-205">响应</span><span class="sxs-lookup"><span data-stu-id="a727f-205">Response</span></span>
<span data-ttu-id="a727f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a727f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





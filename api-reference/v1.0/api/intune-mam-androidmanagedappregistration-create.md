---
title: 创建 androidManagedAppRegistration
description: 创建新的 androidManagedAppRegistration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d80adb9ccd1a5aa235c9ad6f3c64490bc8f2264
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988187"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="cba10-103">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cba10-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="cba10-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cba10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba10-105">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cba10-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cba10-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cba10-106">Prerequisites</span></span>
<span data-ttu-id="cba10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cba10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba10-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cba10-109">Permission type</span></span>|<span data-ttu-id="cba10-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cba10-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cba10-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cba10-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cba10-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba10-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cba10-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cba10-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cba10-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba10-114">Not supported.</span></span>|
|<span data-ttu-id="cba10-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cba10-115">Application</span></span>|<span data-ttu-id="cba10-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba10-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cba10-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cba10-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="cba10-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cba10-118">Request headers</span></span>
|<span data-ttu-id="cba10-119">标头</span><span class="sxs-lookup"><span data-stu-id="cba10-119">Header</span></span>|<span data-ttu-id="cba10-120">值</span><span class="sxs-lookup"><span data-stu-id="cba10-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cba10-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba10-121">Authorization</span></span>|<span data-ttu-id="cba10-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cba10-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cba10-123">接受</span><span class="sxs-lookup"><span data-stu-id="cba10-123">Accept</span></span>|<span data-ttu-id="cba10-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cba10-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba10-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cba10-125">Request body</span></span>
<span data-ttu-id="cba10-126">在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cba10-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="cba10-127">下表显示了创建 androidManagedAppRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cba10-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="cba10-128">属性</span><span class="sxs-lookup"><span data-stu-id="cba10-128">Property</span></span>|<span data-ttu-id="cba10-129">类型</span><span class="sxs-lookup"><span data-stu-id="cba10-129">Type</span></span>|<span data-ttu-id="cba10-130">说明</span><span class="sxs-lookup"><span data-stu-id="cba10-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba10-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cba10-131">createdDateTime</span></span>|<span data-ttu-id="cba10-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cba10-132">DateTimeOffset</span></span>|<span data-ttu-id="cba10-133">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cba10-134">lastSyncDateTime</span></span>|<span data-ttu-id="cba10-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cba10-135">DateTimeOffset</span></span>|<span data-ttu-id="cba10-136">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cba10-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="cba10-137">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="cba10-138">applicationVersion</span></span>|<span data-ttu-id="cba10-139">String</span><span class="sxs-lookup"><span data-stu-id="cba10-139">String</span></span>|<span data-ttu-id="cba10-140">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="cba10-141">managementSdkVersion</span></span>|<span data-ttu-id="cba10-142">String</span><span class="sxs-lookup"><span data-stu-id="cba10-142">String</span></span>|<span data-ttu-id="cba10-143">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="cba10-144">platformVersion</span></span>|<span data-ttu-id="cba10-145">String</span><span class="sxs-lookup"><span data-stu-id="cba10-145">String</span></span>|<span data-ttu-id="cba10-146">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="cba10-147">deviceType</span></span>|<span data-ttu-id="cba10-148">String</span><span class="sxs-lookup"><span data-stu-id="cba10-148">String</span></span>|<span data-ttu-id="cba10-149">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="cba10-150">deviceTag</span></span>|<span data-ttu-id="cba10-151">String</span><span class="sxs-lookup"><span data-stu-id="cba10-151">String</span></span>|<span data-ttu-id="cba10-152">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="cba10-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="cba10-153">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="cba10-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="cba10-154">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="cba10-155">deviceName</span></span>|<span data-ttu-id="cba10-156">String</span><span class="sxs-lookup"><span data-stu-id="cba10-156">String</span></span>|<span data-ttu-id="cba10-157">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="cba10-158">flaggedReasons</span></span>|<span data-ttu-id="cba10-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="cba10-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="cba10-160">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="cba10-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="cba10-161">例如，</span><span class="sxs-lookup"><span data-stu-id="cba10-161">E.g.</span></span> <span data-ttu-id="cba10-162">在从[managedAppRegistration](../resources/intune-mam-managedappregistration.md)继承的根设备上运行的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cba10-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="cba10-163">可取值为：`none`、`rootedDevice`。</span><span class="sxs-lookup"><span data-stu-id="cba10-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="cba10-164">userId</span><span class="sxs-lookup"><span data-stu-id="cba10-164">userId</span></span>|<span data-ttu-id="cba10-165">String</span><span class="sxs-lookup"><span data-stu-id="cba10-165">String</span></span>|<span data-ttu-id="cba10-166">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cba10-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="cba10-167">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="cba10-168">appIdentifier</span></span>|[<span data-ttu-id="cba10-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cba10-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="cba10-170">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-171">id</span><span class="sxs-lookup"><span data-stu-id="cba10-171">id</span></span>|<span data-ttu-id="cba10-172">String</span><span class="sxs-lookup"><span data-stu-id="cba10-172">String</span></span>|<span data-ttu-id="cba10-173">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cba10-173">Key of the entity.</span></span> <span data-ttu-id="cba10-174">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cba10-175">version</span><span class="sxs-lookup"><span data-stu-id="cba10-175">version</span></span>|<span data-ttu-id="cba10-176">String</span><span class="sxs-lookup"><span data-stu-id="cba10-176">String</span></span>|<span data-ttu-id="cba10-177">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="cba10-177">Version of the entity.</span></span> <span data-ttu-id="cba10-178">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cba10-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cba10-179">响应</span><span class="sxs-lookup"><span data-stu-id="cba10-179">Response</span></span>
<span data-ttu-id="cba10-180">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cba10-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba10-181">示例</span><span class="sxs-lookup"><span data-stu-id="cba10-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="cba10-182">请求</span><span class="sxs-lookup"><span data-stu-id="cba10-182">Request</span></span>
<span data-ttu-id="cba10-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cba10-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="cba10-184">响应</span><span class="sxs-lookup"><span data-stu-id="cba10-184">Response</span></span>
<span data-ttu-id="cba10-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cba10-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

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
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```




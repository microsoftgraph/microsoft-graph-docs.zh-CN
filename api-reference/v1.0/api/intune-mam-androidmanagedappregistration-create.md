---
title: 创建 androidManagedAppRegistration
description: 创建新的 androidManagedAppRegistration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b4b2db4b6b725caddf5323450a993aff685af8e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745441"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="106dc-103">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="106dc-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="106dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="106dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="106dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="106dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="106dc-106">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="106dc-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="106dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="106dc-107">Prerequisites</span></span>
<span data-ttu-id="106dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="106dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="106dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="106dc-110">Permission type</span></span>|<span data-ttu-id="106dc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="106dc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="106dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="106dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="106dc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106dc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="106dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="106dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="106dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="106dc-115">Not supported.</span></span>|
|<span data-ttu-id="106dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="106dc-116">Application</span></span>|<span data-ttu-id="106dc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106dc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="106dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="106dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="106dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="106dc-119">Request headers</span></span>
|<span data-ttu-id="106dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="106dc-120">Header</span></span>|<span data-ttu-id="106dc-121">值</span><span class="sxs-lookup"><span data-stu-id="106dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="106dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="106dc-122">Authorization</span></span>|<span data-ttu-id="106dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="106dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="106dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="106dc-124">Accept</span></span>|<span data-ttu-id="106dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="106dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="106dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="106dc-126">Request body</span></span>
<span data-ttu-id="106dc-127">在请求正文中，提供 androidManagedAppRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="106dc-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="106dc-128">下表显示了创建 androidManagedAppRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="106dc-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="106dc-129">属性</span><span class="sxs-lookup"><span data-stu-id="106dc-129">Property</span></span>|<span data-ttu-id="106dc-130">类型</span><span class="sxs-lookup"><span data-stu-id="106dc-130">Type</span></span>|<span data-ttu-id="106dc-131">说明</span><span class="sxs-lookup"><span data-stu-id="106dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="106dc-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="106dc-132">createdDateTime</span></span>|<span data-ttu-id="106dc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="106dc-133">DateTimeOffset</span></span>|<span data-ttu-id="106dc-134">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="106dc-135">lastSyncDateTime</span></span>|<span data-ttu-id="106dc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="106dc-136">DateTimeOffset</span></span>|<span data-ttu-id="106dc-137">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="106dc-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="106dc-138">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="106dc-139">applicationVersion</span></span>|<span data-ttu-id="106dc-140">String</span><span class="sxs-lookup"><span data-stu-id="106dc-140">String</span></span>|<span data-ttu-id="106dc-141">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="106dc-142">managementSdkVersion</span></span>|<span data-ttu-id="106dc-143">String</span><span class="sxs-lookup"><span data-stu-id="106dc-143">String</span></span>|<span data-ttu-id="106dc-144">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="106dc-145">platformVersion</span></span>|<span data-ttu-id="106dc-146">String</span><span class="sxs-lookup"><span data-stu-id="106dc-146">String</span></span>|<span data-ttu-id="106dc-147">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="106dc-148">deviceType</span></span>|<span data-ttu-id="106dc-149">String</span><span class="sxs-lookup"><span data-stu-id="106dc-149">String</span></span>|<span data-ttu-id="106dc-150">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="106dc-151">deviceTag</span></span>|<span data-ttu-id="106dc-152">String</span><span class="sxs-lookup"><span data-stu-id="106dc-152">String</span></span>|<span data-ttu-id="106dc-153">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="106dc-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="106dc-154">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="106dc-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="106dc-155">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="106dc-156">deviceName</span></span>|<span data-ttu-id="106dc-157">String</span><span class="sxs-lookup"><span data-stu-id="106dc-157">String</span></span>|<span data-ttu-id="106dc-158">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-159">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="106dc-159">flaggedReasons</span></span>|<span data-ttu-id="106dc-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="106dc-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="106dc-161">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="106dc-161">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="106dc-162">例如，</span><span class="sxs-lookup"><span data-stu-id="106dc-162">E.g.</span></span> <span data-ttu-id="106dc-163">在根设备上运行的应用 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)。</span><span class="sxs-lookup"><span data-stu-id="106dc-163">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="106dc-164">可取值为：`none`、`rootedDevice`。</span><span class="sxs-lookup"><span data-stu-id="106dc-164">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="106dc-165">userId</span><span class="sxs-lookup"><span data-stu-id="106dc-165">userId</span></span>|<span data-ttu-id="106dc-166">String</span><span class="sxs-lookup"><span data-stu-id="106dc-166">String</span></span>|<span data-ttu-id="106dc-167">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="106dc-167">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="106dc-168">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-169">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="106dc-169">appIdentifier</span></span>|[<span data-ttu-id="106dc-170">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="106dc-170">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="106dc-171">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-171">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-172">id</span><span class="sxs-lookup"><span data-stu-id="106dc-172">id</span></span>|<span data-ttu-id="106dc-173">String</span><span class="sxs-lookup"><span data-stu-id="106dc-173">String</span></span>|<span data-ttu-id="106dc-174">实体的键。</span><span class="sxs-lookup"><span data-stu-id="106dc-174">Key of the entity.</span></span> <span data-ttu-id="106dc-175">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-175">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="106dc-176">version</span><span class="sxs-lookup"><span data-stu-id="106dc-176">version</span></span>|<span data-ttu-id="106dc-177">String</span><span class="sxs-lookup"><span data-stu-id="106dc-177">String</span></span>|<span data-ttu-id="106dc-178">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="106dc-178">Version of the entity.</span></span> <span data-ttu-id="106dc-179">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="106dc-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="106dc-180">响应</span><span class="sxs-lookup"><span data-stu-id="106dc-180">Response</span></span>
<span data-ttu-id="106dc-181">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="106dc-181">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="106dc-182">示例</span><span class="sxs-lookup"><span data-stu-id="106dc-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="106dc-183">请求</span><span class="sxs-lookup"><span data-stu-id="106dc-183">Request</span></span>
<span data-ttu-id="106dc-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="106dc-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="106dc-185">响应</span><span class="sxs-lookup"><span data-stu-id="106dc-185">Response</span></span>
<span data-ttu-id="106dc-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="106dc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





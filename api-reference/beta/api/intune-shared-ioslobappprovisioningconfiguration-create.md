---
title: 创建 iosLobAppProvisioningConfiguration
description: 创建新的 iosLobAppProvisioningConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35d2d18ded6a4dc24a31fc59b2ac37a899c329a2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085932"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="1c457-103">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c457-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="1c457-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c457-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c457-106">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c457-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c457-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c457-107">Prerequisites</span></span>
<span data-ttu-id="1c457-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c457-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c457-110">Permission type</span></span>|<span data-ttu-id="1c457-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c457-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c457-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c457-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1c457-113">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="1c457-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="1c457-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c457-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1c457-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1c457-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1c457-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c457-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c457-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c457-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c457-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c457-118">Not supported.</span></span>|
|<span data-ttu-id="1c457-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c457-119">Application</span></span>||
| <span data-ttu-id="1c457-120">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="1c457-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="1c457-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c457-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1c457-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1c457-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1c457-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c457-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c457-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c457-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c457-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c457-125">Request headers</span></span>
|<span data-ttu-id="1c457-126">标头</span><span class="sxs-lookup"><span data-stu-id="1c457-126">Header</span></span>|<span data-ttu-id="1c457-127">值</span><span class="sxs-lookup"><span data-stu-id="1c457-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c457-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c457-128">Authorization</span></span>|<span data-ttu-id="1c457-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c457-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c457-130">接受</span><span class="sxs-lookup"><span data-stu-id="1c457-130">Accept</span></span>|<span data-ttu-id="1c457-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1c457-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c457-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c457-132">Request body</span></span>
<span data-ttu-id="1c457-133">在请求正文中，提供 iosLobAppProvisioningConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c457-133">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="1c457-134">下表显示创建 iosLobAppProvisioningConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c457-134">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="1c457-135">属性</span><span class="sxs-lookup"><span data-stu-id="1c457-135">Property</span></span>|<span data-ttu-id="1c457-136">类型</span><span class="sxs-lookup"><span data-stu-id="1c457-136">Type</span></span>|<span data-ttu-id="1c457-137">描述</span><span class="sxs-lookup"><span data-stu-id="1c457-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c457-138">id</span><span class="sxs-lookup"><span data-stu-id="1c457-138">id</span></span>|<span data-ttu-id="1c457-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1c457-139">String</span></span>|<span data-ttu-id="1c457-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1c457-140">Key of the entity.</span></span>|
|<span data-ttu-id="1c457-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1c457-141">expirationDateTime</span></span>|<span data-ttu-id="1c457-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c457-142">DateTimeOffset</span></span>|<span data-ttu-id="1c457-143">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1c457-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="1c457-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="1c457-144">payloadFileName</span></span>|<span data-ttu-id="1c457-145">String</span><span class="sxs-lookup"><span data-stu-id="1c457-145">String</span></span>|<span data-ttu-id="1c457-146">有效负载文件名（\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="1c457-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="1c457-147">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="1c457-147">\*.xml).</span></span>|
|<span data-ttu-id="1c457-148">payload</span><span class="sxs-lookup"><span data-stu-id="1c457-148">payload</span></span>|<span data-ttu-id="1c457-149">Binary</span><span class="sxs-lookup"><span data-stu-id="1c457-149">Binary</span></span>|<span data-ttu-id="1c457-150">有效负载。</span><span class="sxs-lookup"><span data-stu-id="1c457-150">Payload.</span></span> <span data-ttu-id="1c457-151">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="1c457-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="1c457-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c457-152">roleScopeTagIds</span></span>|<span data-ttu-id="1c457-153">String collection</span><span class="sxs-lookup"><span data-stu-id="1c457-153">String collection</span></span>|<span data-ttu-id="1c457-154">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="1c457-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="1c457-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c457-155">createdDateTime</span></span>|<span data-ttu-id="1c457-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c457-156">DateTimeOffset</span></span>|<span data-ttu-id="1c457-157">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c457-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="1c457-158">说明</span><span class="sxs-lookup"><span data-stu-id="1c457-158">description</span></span>|<span data-ttu-id="1c457-159">String</span><span class="sxs-lookup"><span data-stu-id="1c457-159">String</span></span>|<span data-ttu-id="1c457-160">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="1c457-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="1c457-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c457-161">lastModifiedDateTime</span></span>|<span data-ttu-id="1c457-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c457-162">DateTimeOffset</span></span>|<span data-ttu-id="1c457-163">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c457-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1c457-164">displayName</span><span class="sxs-lookup"><span data-stu-id="1c457-164">displayName</span></span>|<span data-ttu-id="1c457-165">String</span><span class="sxs-lookup"><span data-stu-id="1c457-165">String</span></span>|<span data-ttu-id="1c457-166">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="1c457-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="1c457-167">version</span><span class="sxs-lookup"><span data-stu-id="1c457-167">version</span></span>|<span data-ttu-id="1c457-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1c457-168">Int32</span></span>|<span data-ttu-id="1c457-169">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1c457-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="1c457-170">响应</span><span class="sxs-lookup"><span data-stu-id="1c457-170">Response</span></span>
<span data-ttu-id="1c457-171">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c457-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c457-172">示例</span><span class="sxs-lookup"><span data-stu-id="1c457-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c457-173">请求</span><span class="sxs-lookup"><span data-stu-id="1c457-173">Request</span></span>
<span data-ttu-id="1c457-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c457-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="1c457-175">响应</span><span class="sxs-lookup"><span data-stu-id="1c457-175">Response</span></span>
<span data-ttu-id="1c457-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c457-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```










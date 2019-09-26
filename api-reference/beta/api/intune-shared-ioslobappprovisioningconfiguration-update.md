---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6d1d4fde8206eb994eca7b24698b69d3392a285
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199879"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="bfc4e-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfc4e-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="bfc4e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfc4e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfc4e-106">更新[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfc4e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfc4e-107">Prerequisites</span></span>
<span data-ttu-id="bfc4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfc4e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfc4e-110">Permission type</span></span>|<span data-ttu-id="bfc4e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfc4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfc4e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc4e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bfc4e-113">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="bfc4e-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bfc4e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc4e-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="bfc4e-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="bfc4e-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bfc4e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc4e-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfc4e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc4e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfc4e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-118">Not supported.</span></span>|
|<span data-ttu-id="bfc4e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfc4e-119">Application</span></span>||
| <span data-ttu-id="bfc4e-120">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="bfc4e-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bfc4e-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc4e-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="bfc4e-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="bfc4e-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bfc4e-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc4e-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfc4e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfc4e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bfc4e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfc4e-125">Request headers</span></span>
|<span data-ttu-id="bfc4e-126">标头</span><span class="sxs-lookup"><span data-stu-id="bfc4e-126">Header</span></span>|<span data-ttu-id="bfc4e-127">值</span><span class="sxs-lookup"><span data-stu-id="bfc4e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfc4e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc4e-128">Authorization</span></span>|<span data-ttu-id="bfc4e-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfc4e-130">接受</span><span class="sxs-lookup"><span data-stu-id="bfc4e-130">Accept</span></span>|<span data-ttu-id="bfc4e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bfc4e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfc4e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfc4e-132">Request body</span></span>
<span data-ttu-id="bfc4e-133">在请求正文中，提供[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-133">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="bfc4e-134">下表显示创建[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-134">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="bfc4e-135">属性</span><span class="sxs-lookup"><span data-stu-id="bfc4e-135">Property</span></span>|<span data-ttu-id="bfc4e-136">类型</span><span class="sxs-lookup"><span data-stu-id="bfc4e-136">Type</span></span>|<span data-ttu-id="bfc4e-137">说明</span><span class="sxs-lookup"><span data-stu-id="bfc4e-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfc4e-138">id</span><span class="sxs-lookup"><span data-stu-id="bfc4e-138">id</span></span>|<span data-ttu-id="bfc4e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bfc4e-139">String</span></span>|<span data-ttu-id="bfc4e-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-140">Key of the entity.</span></span>|
|<span data-ttu-id="bfc4e-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfc4e-141">expirationDateTime</span></span>|<span data-ttu-id="bfc4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfc4e-142">DateTimeOffset</span></span>|<span data-ttu-id="bfc4e-143">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="bfc4e-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="bfc4e-144">payloadFileName</span></span>|<span data-ttu-id="bfc4e-145">String</span><span class="sxs-lookup"><span data-stu-id="bfc4e-145">String</span></span>|<span data-ttu-id="bfc4e-146">有效负载文件名（\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="bfc4e-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="bfc4e-147">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-147">\*.xml).</span></span>|
|<span data-ttu-id="bfc4e-148">payload</span><span class="sxs-lookup"><span data-stu-id="bfc4e-148">payload</span></span>|<span data-ttu-id="bfc4e-149">Binary</span><span class="sxs-lookup"><span data-stu-id="bfc4e-149">Binary</span></span>|<span data-ttu-id="bfc4e-150">有效负载。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-150">Payload.</span></span> <span data-ttu-id="bfc4e-151">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="bfc4e-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="bfc4e-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bfc4e-152">roleScopeTagIds</span></span>|<span data-ttu-id="bfc4e-153">String collection</span><span class="sxs-lookup"><span data-stu-id="bfc4e-153">String collection</span></span>|<span data-ttu-id="bfc4e-154">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="bfc4e-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfc4e-155">createdDateTime</span></span>|<span data-ttu-id="bfc4e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfc4e-156">DateTimeOffset</span></span>|<span data-ttu-id="bfc4e-157">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="bfc4e-158">说明</span><span class="sxs-lookup"><span data-stu-id="bfc4e-158">description</span></span>|<span data-ttu-id="bfc4e-159">String</span><span class="sxs-lookup"><span data-stu-id="bfc4e-159">String</span></span>|<span data-ttu-id="bfc4e-160">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="bfc4e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfc4e-161">lastModifiedDateTime</span></span>|<span data-ttu-id="bfc4e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfc4e-162">DateTimeOffset</span></span>|<span data-ttu-id="bfc4e-163">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bfc4e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="bfc4e-164">displayName</span></span>|<span data-ttu-id="bfc4e-165">String</span><span class="sxs-lookup"><span data-stu-id="bfc4e-165">String</span></span>|<span data-ttu-id="bfc4e-166">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="bfc4e-167">version</span><span class="sxs-lookup"><span data-stu-id="bfc4e-167">version</span></span>|<span data-ttu-id="bfc4e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bfc4e-168">Int32</span></span>|<span data-ttu-id="bfc4e-169">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="bfc4e-170">响应</span><span class="sxs-lookup"><span data-stu-id="bfc4e-170">Response</span></span>
<span data-ttu-id="bfc4e-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfc4e-172">示例</span><span class="sxs-lookup"><span data-stu-id="bfc4e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfc4e-173">请求</span><span class="sxs-lookup"><span data-stu-id="bfc4e-173">Request</span></span>
<span data-ttu-id="bfc4e-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
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

### <a name="response"></a><span data-ttu-id="bfc4e-175">响应</span><span class="sxs-lookup"><span data-stu-id="bfc4e-175">Response</span></span>
<span data-ttu-id="bfc4e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfc4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





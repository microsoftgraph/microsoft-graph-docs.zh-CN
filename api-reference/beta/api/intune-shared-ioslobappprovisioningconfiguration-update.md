---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8021e5a146db9ccc3e275b28228a060cf41b4dd9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217541"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c5f56-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5f56-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="c5f56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5f56-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5f56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f56-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5f56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f56-107">更新 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5f56-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5f56-108">Prerequisites</span></span>
<span data-ttu-id="c5f56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5f56-111">Permission type</span></span>|<span data-ttu-id="c5f56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5f56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5f56-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c5f56-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="c5f56-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c5f56-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f56-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c5f56-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="c5f56-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c5f56-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f56-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5f56-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5f56-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f56-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5f56-119">Not supported.</span></span>|
|<span data-ttu-id="c5f56-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5f56-120">Application</span></span>||
| <span data-ttu-id="c5f56-121">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="c5f56-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c5f56-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f56-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c5f56-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="c5f56-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c5f56-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f56-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f56-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5f56-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5f56-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5f56-126">Request headers</span></span>
|<span data-ttu-id="c5f56-127">标头</span><span class="sxs-lookup"><span data-stu-id="c5f56-127">Header</span></span>|<span data-ttu-id="c5f56-128">值</span><span class="sxs-lookup"><span data-stu-id="c5f56-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f56-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f56-129">Authorization</span></span>|<span data-ttu-id="c5f56-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5f56-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f56-131">接受</span><span class="sxs-lookup"><span data-stu-id="c5f56-131">Accept</span></span>|<span data-ttu-id="c5f56-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f56-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f56-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5f56-133">Request body</span></span>
<span data-ttu-id="c5f56-134">在请求正文中，提供 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5f56-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="c5f56-135">下表显示创建 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5f56-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="c5f56-136">属性</span><span class="sxs-lookup"><span data-stu-id="c5f56-136">Property</span></span>|<span data-ttu-id="c5f56-137">类型</span><span class="sxs-lookup"><span data-stu-id="c5f56-137">Type</span></span>|<span data-ttu-id="c5f56-138">说明</span><span class="sxs-lookup"><span data-stu-id="c5f56-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f56-139">id</span><span class="sxs-lookup"><span data-stu-id="c5f56-139">id</span></span>|<span data-ttu-id="c5f56-140">String</span><span class="sxs-lookup"><span data-stu-id="c5f56-140">String</span></span>|<span data-ttu-id="c5f56-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5f56-141">Key of the entity.</span></span>|
|<span data-ttu-id="c5f56-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f56-142">expirationDateTime</span></span>|<span data-ttu-id="c5f56-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f56-143">DateTimeOffset</span></span>|<span data-ttu-id="c5f56-144">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c5f56-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="c5f56-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c5f56-145">payloadFileName</span></span>|<span data-ttu-id="c5f56-146">String</span><span class="sxs-lookup"><span data-stu-id="c5f56-146">String</span></span>|<span data-ttu-id="c5f56-147">有效负载文件名 ( \* mobileprovision</span><span class="sxs-lookup"><span data-stu-id="c5f56-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="c5f56-148">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="c5f56-148">\*.xml).</span></span>|
|<span data-ttu-id="c5f56-149">payload</span><span class="sxs-lookup"><span data-stu-id="c5f56-149">payload</span></span>|<span data-ttu-id="c5f56-150">Binary</span><span class="sxs-lookup"><span data-stu-id="c5f56-150">Binary</span></span>|<span data-ttu-id="c5f56-151">有效负载。</span><span class="sxs-lookup"><span data-stu-id="c5f56-151">Payload.</span></span> <span data-ttu-id="c5f56-152">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="c5f56-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c5f56-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5f56-153">roleScopeTagIds</span></span>|<span data-ttu-id="c5f56-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="c5f56-154">String collection</span></span>|<span data-ttu-id="c5f56-155">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="c5f56-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="c5f56-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f56-156">createdDateTime</span></span>|<span data-ttu-id="c5f56-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f56-157">DateTimeOffset</span></span>|<span data-ttu-id="c5f56-158">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5f56-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="c5f56-159">description</span><span class="sxs-lookup"><span data-stu-id="c5f56-159">description</span></span>|<span data-ttu-id="c5f56-160">String</span><span class="sxs-lookup"><span data-stu-id="c5f56-160">String</span></span>|<span data-ttu-id="c5f56-161">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="c5f56-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c5f56-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f56-162">lastModifiedDateTime</span></span>|<span data-ttu-id="c5f56-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f56-163">DateTimeOffset</span></span>|<span data-ttu-id="c5f56-164">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5f56-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c5f56-165">displayName</span><span class="sxs-lookup"><span data-stu-id="c5f56-165">displayName</span></span>|<span data-ttu-id="c5f56-166">String</span><span class="sxs-lookup"><span data-stu-id="c5f56-166">String</span></span>|<span data-ttu-id="c5f56-167">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="c5f56-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c5f56-168">version</span><span class="sxs-lookup"><span data-stu-id="c5f56-168">version</span></span>|<span data-ttu-id="c5f56-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f56-169">Int32</span></span>|<span data-ttu-id="c5f56-170">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c5f56-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c5f56-171">响应</span><span class="sxs-lookup"><span data-stu-id="c5f56-171">Response</span></span>
<span data-ttu-id="c5f56-172">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5f56-172">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f56-173">示例</span><span class="sxs-lookup"><span data-stu-id="c5f56-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f56-174">请求</span><span class="sxs-lookup"><span data-stu-id="c5f56-174">Request</span></span>
<span data-ttu-id="c5f56-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5f56-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5f56-176">响应</span><span class="sxs-lookup"><span data-stu-id="c5f56-176">Response</span></span>
<span data-ttu-id="c5f56-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5f56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








---
title: 创建 iosLobAppProvisioningConfiguration
description: 创建新的 iosLobAppProvisioningConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c10a865f1fceabbab22f96216d9ff8c4eabbf25e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729936"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="d9693-103">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9693-103">Create iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="d9693-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9693-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9693-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9693-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9693-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9693-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9693-107">创建新的 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9693-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9693-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9693-108">Prerequisites</span></span>
<span data-ttu-id="d9693-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9693-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9693-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9693-111">Permission type</span></span>|<span data-ttu-id="d9693-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9693-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9693-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9693-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d9693-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d9693-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d9693-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9693-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d9693-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="d9693-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d9693-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9693-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9693-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9693-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9693-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9693-119">Not supported.</span></span>|
|<span data-ttu-id="d9693-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9693-120">Application</span></span>||
| <span data-ttu-id="d9693-121">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d9693-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d9693-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9693-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d9693-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="d9693-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d9693-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9693-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9693-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9693-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9693-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9693-126">Request headers</span></span>
|<span data-ttu-id="d9693-127">标头</span><span class="sxs-lookup"><span data-stu-id="d9693-127">Header</span></span>|<span data-ttu-id="d9693-128">值</span><span class="sxs-lookup"><span data-stu-id="d9693-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9693-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9693-129">Authorization</span></span>|<span data-ttu-id="d9693-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9693-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9693-131">接受</span><span class="sxs-lookup"><span data-stu-id="d9693-131">Accept</span></span>|<span data-ttu-id="d9693-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d9693-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9693-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9693-133">Request body</span></span>
<span data-ttu-id="d9693-134">在请求正文中，提供 iosLobAppProvisioningConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9693-134">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="d9693-135">下表显示创建 iosLobAppProvisioningConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9693-135">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="d9693-136">属性</span><span class="sxs-lookup"><span data-stu-id="d9693-136">Property</span></span>|<span data-ttu-id="d9693-137">类型</span><span class="sxs-lookup"><span data-stu-id="d9693-137">Type</span></span>|<span data-ttu-id="d9693-138">说明</span><span class="sxs-lookup"><span data-stu-id="d9693-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9693-139">id</span><span class="sxs-lookup"><span data-stu-id="d9693-139">id</span></span>|<span data-ttu-id="d9693-140">String</span><span class="sxs-lookup"><span data-stu-id="d9693-140">String</span></span>|<span data-ttu-id="d9693-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9693-141">Key of the entity.</span></span>|
|<span data-ttu-id="d9693-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9693-142">expirationDateTime</span></span>|<span data-ttu-id="d9693-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9693-143">DateTimeOffset</span></span>|<span data-ttu-id="d9693-144">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9693-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="d9693-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d9693-145">payloadFileName</span></span>|<span data-ttu-id="d9693-146">String</span><span class="sxs-lookup"><span data-stu-id="d9693-146">String</span></span>|<span data-ttu-id="d9693-147">有效负载文件名 ( \* mobileprovision</span><span class="sxs-lookup"><span data-stu-id="d9693-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="d9693-148">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="d9693-148">\*.xml).</span></span>|
|<span data-ttu-id="d9693-149">payload</span><span class="sxs-lookup"><span data-stu-id="d9693-149">payload</span></span>|<span data-ttu-id="d9693-150">Binary</span><span class="sxs-lookup"><span data-stu-id="d9693-150">Binary</span></span>|<span data-ttu-id="d9693-151">有效负载。</span><span class="sxs-lookup"><span data-stu-id="d9693-151">Payload.</span></span> <span data-ttu-id="d9693-152">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="d9693-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="d9693-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9693-153">roleScopeTagIds</span></span>|<span data-ttu-id="d9693-154">String collection</span><span class="sxs-lookup"><span data-stu-id="d9693-154">String collection</span></span>|<span data-ttu-id="d9693-155">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="d9693-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="d9693-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9693-156">createdDateTime</span></span>|<span data-ttu-id="d9693-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9693-157">DateTimeOffset</span></span>|<span data-ttu-id="d9693-158">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9693-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="d9693-159">说明</span><span class="sxs-lookup"><span data-stu-id="d9693-159">description</span></span>|<span data-ttu-id="d9693-160">String</span><span class="sxs-lookup"><span data-stu-id="d9693-160">String</span></span>|<span data-ttu-id="d9693-161">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="d9693-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d9693-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9693-162">lastModifiedDateTime</span></span>|<span data-ttu-id="d9693-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9693-163">DateTimeOffset</span></span>|<span data-ttu-id="d9693-164">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9693-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d9693-165">displayName</span><span class="sxs-lookup"><span data-stu-id="d9693-165">displayName</span></span>|<span data-ttu-id="d9693-166">String</span><span class="sxs-lookup"><span data-stu-id="d9693-166">String</span></span>|<span data-ttu-id="d9693-167">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="d9693-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d9693-168">version</span><span class="sxs-lookup"><span data-stu-id="d9693-168">version</span></span>|<span data-ttu-id="d9693-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d9693-169">Int32</span></span>|<span data-ttu-id="d9693-170">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d9693-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d9693-171">响应</span><span class="sxs-lookup"><span data-stu-id="d9693-171">Response</span></span>
<span data-ttu-id="d9693-172">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9693-172">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9693-173">示例</span><span class="sxs-lookup"><span data-stu-id="d9693-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9693-174">请求</span><span class="sxs-lookup"><span data-stu-id="d9693-174">Request</span></span>
<span data-ttu-id="d9693-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9693-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9693-176">响应</span><span class="sxs-lookup"><span data-stu-id="d9693-176">Response</span></span>
<span data-ttu-id="d9693-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9693-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









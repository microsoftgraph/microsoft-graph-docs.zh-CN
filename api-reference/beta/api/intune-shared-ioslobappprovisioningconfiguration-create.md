---
title: 创建 iosLobAppProvisioningConfiguration
description: 创建新的 iosLobAppProvisioningConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c78f8307ce3418b1bb27920b694ac87131023bd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867719"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="ea0b2-103">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea0b2-103">Create iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="ea0b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea0b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea0b2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea0b2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea0b2-107">创建新的 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea0b2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea0b2-108">Prerequisites</span></span>
<span data-ttu-id="ea0b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea0b2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea0b2-111">Permission type</span></span>|<span data-ttu-id="ea0b2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea0b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea0b2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea0b2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea0b2-114">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="ea0b2-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ea0b2-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea0b2-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ea0b2-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ea0b2-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ea0b2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea0b2-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea0b2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea0b2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea0b2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-119">Not supported.</span></span>|
|<span data-ttu-id="ea0b2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea0b2-120">Application</span></span>||
| <span data-ttu-id="ea0b2-121">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="ea0b2-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ea0b2-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea0b2-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ea0b2-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ea0b2-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ea0b2-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea0b2-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea0b2-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea0b2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea0b2-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea0b2-126">Request headers</span></span>
|<span data-ttu-id="ea0b2-127">标头</span><span class="sxs-lookup"><span data-stu-id="ea0b2-127">Header</span></span>|<span data-ttu-id="ea0b2-128">值</span><span class="sxs-lookup"><span data-stu-id="ea0b2-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea0b2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea0b2-129">Authorization</span></span>|<span data-ttu-id="ea0b2-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea0b2-131">接受</span><span class="sxs-lookup"><span data-stu-id="ea0b2-131">Accept</span></span>|<span data-ttu-id="ea0b2-132">application/json</span><span class="sxs-lookup"><span data-stu-id="ea0b2-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea0b2-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea0b2-133">Request body</span></span>
<span data-ttu-id="ea0b2-134">在请求正文中，提供 iosLobAppProvisioningConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-134">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="ea0b2-135">下表显示创建 iosLobAppProvisioningConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-135">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="ea0b2-136">属性</span><span class="sxs-lookup"><span data-stu-id="ea0b2-136">Property</span></span>|<span data-ttu-id="ea0b2-137">类型</span><span class="sxs-lookup"><span data-stu-id="ea0b2-137">Type</span></span>|<span data-ttu-id="ea0b2-138">说明</span><span class="sxs-lookup"><span data-stu-id="ea0b2-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea0b2-139">id</span><span class="sxs-lookup"><span data-stu-id="ea0b2-139">id</span></span>|<span data-ttu-id="ea0b2-140">String</span><span class="sxs-lookup"><span data-stu-id="ea0b2-140">String</span></span>|<span data-ttu-id="ea0b2-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-141">Key of the entity.</span></span>|
|<span data-ttu-id="ea0b2-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea0b2-142">expirationDateTime</span></span>|<span data-ttu-id="ea0b2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea0b2-143">DateTimeOffset</span></span>|<span data-ttu-id="ea0b2-144">可选的配置文件过期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="ea0b2-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ea0b2-145">payloadFileName</span></span>|<span data-ttu-id="ea0b2-146">String</span><span class="sxs-lookup"><span data-stu-id="ea0b2-146">String</span></span>|<span data-ttu-id="ea0b2-147">有效负载文件名 (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="ea0b2-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="ea0b2-148">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-148">\*.xml).</span></span>|
|<span data-ttu-id="ea0b2-149">payload</span><span class="sxs-lookup"><span data-stu-id="ea0b2-149">payload</span></span>|<span data-ttu-id="ea0b2-150">Binary</span><span class="sxs-lookup"><span data-stu-id="ea0b2-150">Binary</span></span>|<span data-ttu-id="ea0b2-151">有效负载。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-151">Payload.</span></span> <span data-ttu-id="ea0b2-152">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="ea0b2-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="ea0b2-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea0b2-153">roleScopeTagIds</span></span>|<span data-ttu-id="ea0b2-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="ea0b2-154">String collection</span></span>|<span data-ttu-id="ea0b2-155">此 iOS LOB 应用预配配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="ea0b2-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea0b2-156">createdDateTime</span></span>|<span data-ttu-id="ea0b2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea0b2-157">DateTimeOffset</span></span>|<span data-ttu-id="ea0b2-158">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="ea0b2-159">说明</span><span class="sxs-lookup"><span data-stu-id="ea0b2-159">description</span></span>|<span data-ttu-id="ea0b2-160">String</span><span class="sxs-lookup"><span data-stu-id="ea0b2-160">String</span></span>|<span data-ttu-id="ea0b2-161">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ea0b2-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea0b2-162">lastModifiedDateTime</span></span>|<span data-ttu-id="ea0b2-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea0b2-163">DateTimeOffset</span></span>|<span data-ttu-id="ea0b2-164">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ea0b2-165">displayName</span><span class="sxs-lookup"><span data-stu-id="ea0b2-165">displayName</span></span>|<span data-ttu-id="ea0b2-166">String</span><span class="sxs-lookup"><span data-stu-id="ea0b2-166">String</span></span>|<span data-ttu-id="ea0b2-167">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ea0b2-168">version</span><span class="sxs-lookup"><span data-stu-id="ea0b2-168">version</span></span>|<span data-ttu-id="ea0b2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ea0b2-169">Int32</span></span>|<span data-ttu-id="ea0b2-170">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ea0b2-171">响应</span><span class="sxs-lookup"><span data-stu-id="ea0b2-171">Response</span></span>
<span data-ttu-id="ea0b2-172">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-172">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea0b2-173">示例</span><span class="sxs-lookup"><span data-stu-id="ea0b2-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea0b2-174">请求</span><span class="sxs-lookup"><span data-stu-id="ea0b2-174">Request</span></span>
<span data-ttu-id="ea0b2-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea0b2-176">响应</span><span class="sxs-lookup"><span data-stu-id="ea0b2-176">Response</span></span>
<span data-ttu-id="ea0b2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea0b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








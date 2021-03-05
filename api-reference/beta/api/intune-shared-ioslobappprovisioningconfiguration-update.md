---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efeecc86bdb481b3b77871551ced12694c3eb590
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471829"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="177cb-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="177cb-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="177cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="177cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="177cb-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="177cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="177cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="177cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="177cb-107">更新 [iosLobAppProvisioningConfiguration 对象](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="177cb-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="177cb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="177cb-108">Prerequisites</span></span>
<span data-ttu-id="177cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="177cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="177cb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="177cb-111">Permission type</span></span>|<span data-ttu-id="177cb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="177cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="177cb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="177cb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="177cb-114">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="177cb-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="177cb-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177cb-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="177cb-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="177cb-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="177cb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177cb-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="177cb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="177cb-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="177cb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="177cb-119">Not supported.</span></span>|
|<span data-ttu-id="177cb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="177cb-120">Application</span></span>||
| <span data-ttu-id="177cb-121">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="177cb-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="177cb-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177cb-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="177cb-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="177cb-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="177cb-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177cb-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="177cb-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="177cb-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="177cb-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="177cb-126">Request headers</span></span>
|<span data-ttu-id="177cb-127">标头</span><span class="sxs-lookup"><span data-stu-id="177cb-127">Header</span></span>|<span data-ttu-id="177cb-128">值</span><span class="sxs-lookup"><span data-stu-id="177cb-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="177cb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="177cb-129">Authorization</span></span>|<span data-ttu-id="177cb-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="177cb-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="177cb-131">接受</span><span class="sxs-lookup"><span data-stu-id="177cb-131">Accept</span></span>|<span data-ttu-id="177cb-132">application/json</span><span class="sxs-lookup"><span data-stu-id="177cb-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="177cb-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="177cb-133">Request body</span></span>
<span data-ttu-id="177cb-134">在请求正文中，提供 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="177cb-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="177cb-135">下表显示创建 [iosLobAppProvisioningConfiguration 时所需的属性](../resources/intune-shared-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="177cb-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="177cb-136">属性</span><span class="sxs-lookup"><span data-stu-id="177cb-136">Property</span></span>|<span data-ttu-id="177cb-137">类型</span><span class="sxs-lookup"><span data-stu-id="177cb-137">Type</span></span>|<span data-ttu-id="177cb-138">说明</span><span class="sxs-lookup"><span data-stu-id="177cb-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="177cb-139">id</span><span class="sxs-lookup"><span data-stu-id="177cb-139">id</span></span>|<span data-ttu-id="177cb-140">String</span><span class="sxs-lookup"><span data-stu-id="177cb-140">String</span></span>|<span data-ttu-id="177cb-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="177cb-141">Key of the entity.</span></span>|
|<span data-ttu-id="177cb-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="177cb-142">expirationDateTime</span></span>|<span data-ttu-id="177cb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177cb-143">DateTimeOffset</span></span>|<span data-ttu-id="177cb-144">可选的配置文件过期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="177cb-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="177cb-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="177cb-145">payloadFileName</span></span>|<span data-ttu-id="177cb-146">String</span><span class="sxs-lookup"><span data-stu-id="177cb-146">String</span></span>|<span data-ttu-id="177cb-147">有效负载文件名 (\*.mobileprovision \| \*.xml) 。</span><span class="sxs-lookup"><span data-stu-id="177cb-147">Payload file name (\*.mobileprovision \| \*.xml).</span></span>|
|<span data-ttu-id="177cb-148">payload</span><span class="sxs-lookup"><span data-stu-id="177cb-148">payload</span></span>|<span data-ttu-id="177cb-149">Binary</span><span class="sxs-lookup"><span data-stu-id="177cb-149">Binary</span></span>|<span data-ttu-id="177cb-150">有效负载。</span><span class="sxs-lookup"><span data-stu-id="177cb-150">Payload.</span></span> <span data-ttu-id="177cb-151">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="177cb-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="177cb-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="177cb-152">roleScopeTagIds</span></span>|<span data-ttu-id="177cb-153">String collection</span><span class="sxs-lookup"><span data-stu-id="177cb-153">String collection</span></span>|<span data-ttu-id="177cb-154">此 iOS LOB 应用预配配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="177cb-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="177cb-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="177cb-155">createdDateTime</span></span>|<span data-ttu-id="177cb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177cb-156">DateTimeOffset</span></span>|<span data-ttu-id="177cb-157">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="177cb-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="177cb-158">说明</span><span class="sxs-lookup"><span data-stu-id="177cb-158">description</span></span>|<span data-ttu-id="177cb-159">String</span><span class="sxs-lookup"><span data-stu-id="177cb-159">String</span></span>|<span data-ttu-id="177cb-160">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="177cb-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="177cb-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="177cb-161">lastModifiedDateTime</span></span>|<span data-ttu-id="177cb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177cb-162">DateTimeOffset</span></span>|<span data-ttu-id="177cb-163">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="177cb-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="177cb-164">displayName</span><span class="sxs-lookup"><span data-stu-id="177cb-164">displayName</span></span>|<span data-ttu-id="177cb-165">String</span><span class="sxs-lookup"><span data-stu-id="177cb-165">String</span></span>|<span data-ttu-id="177cb-166">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="177cb-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="177cb-167">version</span><span class="sxs-lookup"><span data-stu-id="177cb-167">version</span></span>|<span data-ttu-id="177cb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="177cb-168">Int32</span></span>|<span data-ttu-id="177cb-169">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="177cb-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="177cb-170">响应</span><span class="sxs-lookup"><span data-stu-id="177cb-170">Response</span></span>
<span data-ttu-id="177cb-171">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="177cb-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="177cb-172">示例</span><span class="sxs-lookup"><span data-stu-id="177cb-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="177cb-173">请求</span><span class="sxs-lookup"><span data-stu-id="177cb-173">Request</span></span>
<span data-ttu-id="177cb-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="177cb-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="177cb-175">响应</span><span class="sxs-lookup"><span data-stu-id="177cb-175">Response</span></span>
<span data-ttu-id="177cb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="177cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








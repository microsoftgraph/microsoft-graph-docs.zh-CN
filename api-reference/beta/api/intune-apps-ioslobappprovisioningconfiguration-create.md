---
title: 创建 iosLobAppProvisioningConfiguration
description: 创建新的 iosLobAppProvisioningConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d8cf36c1e4fe957d05463df2dae4975f2d07fcb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968656"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="96148-103">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="96148-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="96148-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96148-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96148-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96148-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96148-106">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96148-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96148-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="96148-107">Prerequisites</span></span>
<span data-ttu-id="96148-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96148-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96148-110">Permission type</span></span>|<span data-ttu-id="96148-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96148-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96148-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96148-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96148-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96148-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96148-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96148-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96148-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96148-115">Not supported.</span></span>|
|<span data-ttu-id="96148-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96148-116">Application</span></span>|<span data-ttu-id="96148-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96148-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96148-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96148-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96148-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96148-119">Request headers</span></span>
|<span data-ttu-id="96148-120">标头</span><span class="sxs-lookup"><span data-stu-id="96148-120">Header</span></span>|<span data-ttu-id="96148-121">值</span><span class="sxs-lookup"><span data-stu-id="96148-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96148-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96148-122">Authorization</span></span>|<span data-ttu-id="96148-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96148-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96148-124">接受</span><span class="sxs-lookup"><span data-stu-id="96148-124">Accept</span></span>|<span data-ttu-id="96148-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96148-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96148-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="96148-126">Request body</span></span>
<span data-ttu-id="96148-127">在请求正文中, 提供 iosLobAppProvisioningConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96148-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="96148-128">下表显示创建 iosLobAppProvisioningConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="96148-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="96148-129">属性</span><span class="sxs-lookup"><span data-stu-id="96148-129">Property</span></span>|<span data-ttu-id="96148-130">类型</span><span class="sxs-lookup"><span data-stu-id="96148-130">Type</span></span>|<span data-ttu-id="96148-131">说明</span><span class="sxs-lookup"><span data-stu-id="96148-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96148-132">id</span><span class="sxs-lookup"><span data-stu-id="96148-132">id</span></span>|<span data-ttu-id="96148-133">String</span><span class="sxs-lookup"><span data-stu-id="96148-133">String</span></span>|<span data-ttu-id="96148-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="96148-134">Key of the entity.</span></span>|
|<span data-ttu-id="96148-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="96148-135">expirationDateTime</span></span>|<span data-ttu-id="96148-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96148-136">DateTimeOffset</span></span>|<span data-ttu-id="96148-137">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="96148-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="96148-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="96148-138">payloadFileName</span></span>|<span data-ttu-id="96148-139">String</span><span class="sxs-lookup"><span data-stu-id="96148-139">String</span></span>|<span data-ttu-id="96148-140">有效负载文件名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="96148-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="96148-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="96148-141">\*.xml).</span></span>|
|<span data-ttu-id="96148-142">payload</span><span class="sxs-lookup"><span data-stu-id="96148-142">payload</span></span>|<span data-ttu-id="96148-143">Binary</span><span class="sxs-lookup"><span data-stu-id="96148-143">Binary</span></span>|<span data-ttu-id="96148-144">有效负载。</span><span class="sxs-lookup"><span data-stu-id="96148-144">Payload.</span></span> <span data-ttu-id="96148-145">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="96148-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="96148-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96148-146">roleScopeTagIds</span></span>|<span data-ttu-id="96148-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="96148-147">String collection</span></span>|<span data-ttu-id="96148-148">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="96148-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="96148-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96148-149">createdDateTime</span></span>|<span data-ttu-id="96148-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96148-150">DateTimeOffset</span></span>|<span data-ttu-id="96148-151">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="96148-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="96148-152">description</span><span class="sxs-lookup"><span data-stu-id="96148-152">description</span></span>|<span data-ttu-id="96148-153">String</span><span class="sxs-lookup"><span data-stu-id="96148-153">String</span></span>|<span data-ttu-id="96148-154">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="96148-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="96148-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96148-155">lastModifiedDateTime</span></span>|<span data-ttu-id="96148-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96148-156">DateTimeOffset</span></span>|<span data-ttu-id="96148-157">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="96148-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="96148-158">displayName</span><span class="sxs-lookup"><span data-stu-id="96148-158">displayName</span></span>|<span data-ttu-id="96148-159">String</span><span class="sxs-lookup"><span data-stu-id="96148-159">String</span></span>|<span data-ttu-id="96148-160">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="96148-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="96148-161">version</span><span class="sxs-lookup"><span data-stu-id="96148-161">version</span></span>|<span data-ttu-id="96148-162">Int32</span><span class="sxs-lookup"><span data-stu-id="96148-162">Int32</span></span>|<span data-ttu-id="96148-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="96148-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="96148-164">响应</span><span class="sxs-lookup"><span data-stu-id="96148-164">Response</span></span>
<span data-ttu-id="96148-165">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96148-165">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96148-166">示例</span><span class="sxs-lookup"><span data-stu-id="96148-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="96148-167">请求</span><span class="sxs-lookup"><span data-stu-id="96148-167">Request</span></span>
<span data-ttu-id="96148-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96148-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96148-169">响应</span><span class="sxs-lookup"><span data-stu-id="96148-169">Response</span></span>
<span data-ttu-id="96148-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96148-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





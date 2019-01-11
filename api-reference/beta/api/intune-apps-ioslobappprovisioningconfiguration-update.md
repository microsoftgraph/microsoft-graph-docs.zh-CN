---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 637c1052f4097c3a33ff4c8fc4949ef48773ce68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859316"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="e1fbb-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1fbb-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="e1fbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1fbb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1fbb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1fbb-107">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1fbb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1fbb-108">Prerequisites</span></span>
<span data-ttu-id="e1fbb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e1fbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fbb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1fbb-111">Permission type</span></span>|<span data-ttu-id="e1fbb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e1fbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1fbb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1fbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1fbb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fbb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1fbb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1fbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1fbb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-116">Not supported.</span></span>|
|<span data-ttu-id="e1fbb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1fbb-117">Application</span></span>|<span data-ttu-id="e1fbb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1fbb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1fbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e1fbb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1fbb-120">Request headers</span></span>
|<span data-ttu-id="e1fbb-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1fbb-121">Header</span></span>|<span data-ttu-id="e1fbb-122">值</span><span class="sxs-lookup"><span data-stu-id="e1fbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1fbb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1fbb-123">Authorization</span></span>|<span data-ttu-id="e1fbb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1fbb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1fbb-125">Accept</span></span>|<span data-ttu-id="e1fbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1fbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1fbb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1fbb-127">Request body</span></span>
<span data-ttu-id="e1fbb-128">在请求正文中，提供[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="e1fbb-129">下表显示时创建[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="e1fbb-130">属性</span><span class="sxs-lookup"><span data-stu-id="e1fbb-130">Property</span></span>|<span data-ttu-id="e1fbb-131">类型</span><span class="sxs-lookup"><span data-stu-id="e1fbb-131">Type</span></span>|<span data-ttu-id="e1fbb-132">说明</span><span class="sxs-lookup"><span data-stu-id="e1fbb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1fbb-133">id</span><span class="sxs-lookup"><span data-stu-id="e1fbb-133">id</span></span>|<span data-ttu-id="e1fbb-134">String</span><span class="sxs-lookup"><span data-stu-id="e1fbb-134">String</span></span>|<span data-ttu-id="e1fbb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1fbb-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fbb-136">expirationDateTime</span></span>|<span data-ttu-id="e1fbb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fbb-137">DateTimeOffset</span></span>|<span data-ttu-id="e1fbb-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="e1fbb-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e1fbb-139">payloadFileName</span></span>|<span data-ttu-id="e1fbb-140">String</span><span class="sxs-lookup"><span data-stu-id="e1fbb-140">String</span></span>|<span data-ttu-id="e1fbb-141">负载文件名 (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="e1fbb-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="e1fbb-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-142">\*.xml).</span></span>|
|<span data-ttu-id="e1fbb-143">payload</span><span class="sxs-lookup"><span data-stu-id="e1fbb-143">payload</span></span>|<span data-ttu-id="e1fbb-144">Binary</span><span class="sxs-lookup"><span data-stu-id="e1fbb-144">Binary</span></span>|<span data-ttu-id="e1fbb-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-145">Payload.</span></span> <span data-ttu-id="e1fbb-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="e1fbb-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="e1fbb-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fbb-147">createdDateTime</span></span>|<span data-ttu-id="e1fbb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fbb-148">DateTimeOffset</span></span>|<span data-ttu-id="e1fbb-149">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="e1fbb-150">description</span><span class="sxs-lookup"><span data-stu-id="e1fbb-150">description</span></span>|<span data-ttu-id="e1fbb-151">String</span><span class="sxs-lookup"><span data-stu-id="e1fbb-151">String</span></span>|<span data-ttu-id="e1fbb-152">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="e1fbb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fbb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e1fbb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fbb-154">DateTimeOffset</span></span>|<span data-ttu-id="e1fbb-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e1fbb-156">displayName</span><span class="sxs-lookup"><span data-stu-id="e1fbb-156">displayName</span></span>|<span data-ttu-id="e1fbb-157">String</span><span class="sxs-lookup"><span data-stu-id="e1fbb-157">String</span></span>|<span data-ttu-id="e1fbb-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="e1fbb-159">version</span><span class="sxs-lookup"><span data-stu-id="e1fbb-159">version</span></span>|<span data-ttu-id="e1fbb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e1fbb-160">Int32</span></span>|<span data-ttu-id="e1fbb-161">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="e1fbb-162">响应</span><span class="sxs-lookup"><span data-stu-id="e1fbb-162">Response</span></span>
<span data-ttu-id="e1fbb-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1fbb-164">示例</span><span class="sxs-lookup"><span data-stu-id="e1fbb-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1fbb-165">请求</span><span class="sxs-lookup"><span data-stu-id="e1fbb-165">Request</span></span>
<span data-ttu-id="e1fbb-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 304

{
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="e1fbb-167">响应</span><span class="sxs-lookup"><span data-stu-id="e1fbb-167">Response</span></span>
<span data-ttu-id="e1fbb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1fbb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```






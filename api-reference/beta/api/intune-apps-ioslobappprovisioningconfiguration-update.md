---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 191df244cf163d0a5980c9fc0c5ae3a444e3468c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173085"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="fec54-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="fec54-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="fec54-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fec54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fec54-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fec54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fec54-106">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fec54-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fec54-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fec54-107">Prerequisites</span></span>
<span data-ttu-id="fec54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fec54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fec54-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fec54-110">Permission type</span></span>|<span data-ttu-id="fec54-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fec54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fec54-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fec54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fec54-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fec54-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fec54-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fec54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fec54-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fec54-115">Not supported.</span></span>|
|<span data-ttu-id="fec54-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fec54-116">Application</span></span>|<span data-ttu-id="fec54-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fec54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fec54-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fec54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fec54-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fec54-119">Request headers</span></span>
|<span data-ttu-id="fec54-120">标头</span><span class="sxs-lookup"><span data-stu-id="fec54-120">Header</span></span>|<span data-ttu-id="fec54-121">值</span><span class="sxs-lookup"><span data-stu-id="fec54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fec54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fec54-122">Authorization</span></span>|<span data-ttu-id="fec54-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fec54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fec54-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fec54-124">Accept</span></span>|<span data-ttu-id="fec54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fec54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fec54-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fec54-126">Request body</span></span>
<span data-ttu-id="fec54-127">在请求正文中, 提供[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fec54-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="fec54-128">下表显示创建[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fec54-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="fec54-129">属性</span><span class="sxs-lookup"><span data-stu-id="fec54-129">Property</span></span>|<span data-ttu-id="fec54-130">类型</span><span class="sxs-lookup"><span data-stu-id="fec54-130">Type</span></span>|<span data-ttu-id="fec54-131">说明</span><span class="sxs-lookup"><span data-stu-id="fec54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec54-132">id</span><span class="sxs-lookup"><span data-stu-id="fec54-132">id</span></span>|<span data-ttu-id="fec54-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fec54-133">String</span></span>|<span data-ttu-id="fec54-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fec54-134">Key of the entity.</span></span>|
|<span data-ttu-id="fec54-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fec54-135">expirationDateTime</span></span>|<span data-ttu-id="fec54-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec54-136">DateTimeOffset</span></span>|<span data-ttu-id="fec54-137">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fec54-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="fec54-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="fec54-138">payloadFileName</span></span>|<span data-ttu-id="fec54-139">String</span><span class="sxs-lookup"><span data-stu-id="fec54-139">String</span></span>|<span data-ttu-id="fec54-140">有效负载文件名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="fec54-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="fec54-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="fec54-141">\*.xml).</span></span>|
|<span data-ttu-id="fec54-142">payload</span><span class="sxs-lookup"><span data-stu-id="fec54-142">payload</span></span>|<span data-ttu-id="fec54-143">Binary</span><span class="sxs-lookup"><span data-stu-id="fec54-143">Binary</span></span>|<span data-ttu-id="fec54-144">有效负载。</span><span class="sxs-lookup"><span data-stu-id="fec54-144">Payload.</span></span> <span data-ttu-id="fec54-145">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="fec54-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="fec54-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fec54-146">createdDateTime</span></span>|<span data-ttu-id="fec54-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec54-147">DateTimeOffset</span></span>|<span data-ttu-id="fec54-148">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fec54-148">DateTime the object was created.</span></span>|
|<span data-ttu-id="fec54-149">description</span><span class="sxs-lookup"><span data-stu-id="fec54-149">description</span></span>|<span data-ttu-id="fec54-150">String</span><span class="sxs-lookup"><span data-stu-id="fec54-150">String</span></span>|<span data-ttu-id="fec54-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="fec54-151">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="fec54-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fec54-152">lastModifiedDateTime</span></span>|<span data-ttu-id="fec54-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec54-153">DateTimeOffset</span></span>|<span data-ttu-id="fec54-154">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fec54-154">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fec54-155">displayName</span><span class="sxs-lookup"><span data-stu-id="fec54-155">displayName</span></span>|<span data-ttu-id="fec54-156">String</span><span class="sxs-lookup"><span data-stu-id="fec54-156">String</span></span>|<span data-ttu-id="fec54-157">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="fec54-157">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="fec54-158">version</span><span class="sxs-lookup"><span data-stu-id="fec54-158">version</span></span>|<span data-ttu-id="fec54-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fec54-159">Int32</span></span>|<span data-ttu-id="fec54-160">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fec54-160">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fec54-161">响应</span><span class="sxs-lookup"><span data-stu-id="fec54-161">Response</span></span>
<span data-ttu-id="fec54-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fec54-162">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fec54-163">示例</span><span class="sxs-lookup"><span data-stu-id="fec54-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="fec54-164">请求</span><span class="sxs-lookup"><span data-stu-id="fec54-164">Request</span></span>
<span data-ttu-id="fec54-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fec54-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="fec54-166">响应</span><span class="sxs-lookup"><span data-stu-id="fec54-166">Response</span></span>
<span data-ttu-id="fec54-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fec54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





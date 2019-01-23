---
title: 更新 iosLobAppProvisioningConfiguration
description: 更新 iosLobAppProvisioningConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d98e19b922b1fd9cd2c9205eae89c0637dca9436
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402669"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="2c497-103">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c497-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="2c497-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2c497-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c497-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c497-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c497-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c497-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c497-107">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c497-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c497-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c497-108">Prerequisites</span></span>
<span data-ttu-id="2c497-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c497-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2c497-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c497-111">Permission type</span></span>|<span data-ttu-id="2c497-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c497-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c497-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c497-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c497-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c497-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c497-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c497-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c497-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c497-116">Not supported.</span></span>|
|<span data-ttu-id="2c497-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c497-117">Application</span></span>|<span data-ttu-id="2c497-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c497-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c497-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c497-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2c497-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c497-120">Request headers</span></span>
|<span data-ttu-id="2c497-121">标头</span><span class="sxs-lookup"><span data-stu-id="2c497-121">Header</span></span>|<span data-ttu-id="2c497-122">值</span><span class="sxs-lookup"><span data-stu-id="2c497-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c497-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c497-123">Authorization</span></span>|<span data-ttu-id="2c497-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c497-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c497-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c497-125">Accept</span></span>|<span data-ttu-id="2c497-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c497-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c497-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c497-127">Request body</span></span>
<span data-ttu-id="2c497-128">在请求正文中，提供[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c497-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="2c497-129">下表显示时创建[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c497-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="2c497-130">属性</span><span class="sxs-lookup"><span data-stu-id="2c497-130">Property</span></span>|<span data-ttu-id="2c497-131">类型</span><span class="sxs-lookup"><span data-stu-id="2c497-131">Type</span></span>|<span data-ttu-id="2c497-132">说明</span><span class="sxs-lookup"><span data-stu-id="2c497-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c497-133">id</span><span class="sxs-lookup"><span data-stu-id="2c497-133">id</span></span>|<span data-ttu-id="2c497-134">String</span><span class="sxs-lookup"><span data-stu-id="2c497-134">String</span></span>|<span data-ttu-id="2c497-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2c497-135">Key of the entity.</span></span>|
|<span data-ttu-id="2c497-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2c497-136">expirationDateTime</span></span>|<span data-ttu-id="2c497-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c497-137">DateTimeOffset</span></span>|<span data-ttu-id="2c497-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2c497-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="2c497-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2c497-139">payloadFileName</span></span>|<span data-ttu-id="2c497-140">String</span><span class="sxs-lookup"><span data-stu-id="2c497-140">String</span></span>|<span data-ttu-id="2c497-141">负载文件名 (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="2c497-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="2c497-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="2c497-142">\*.xml).</span></span>|
|<span data-ttu-id="2c497-143">payload</span><span class="sxs-lookup"><span data-stu-id="2c497-143">payload</span></span>|<span data-ttu-id="2c497-144">Binary</span><span class="sxs-lookup"><span data-stu-id="2c497-144">Binary</span></span>|<span data-ttu-id="2c497-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="2c497-145">Payload.</span></span> <span data-ttu-id="2c497-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="2c497-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="2c497-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c497-147">createdDateTime</span></span>|<span data-ttu-id="2c497-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c497-148">DateTimeOffset</span></span>|<span data-ttu-id="2c497-149">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c497-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="2c497-150">description</span><span class="sxs-lookup"><span data-stu-id="2c497-150">description</span></span>|<span data-ttu-id="2c497-151">String</span><span class="sxs-lookup"><span data-stu-id="2c497-151">String</span></span>|<span data-ttu-id="2c497-152">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="2c497-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="2c497-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c497-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2c497-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c497-154">DateTimeOffset</span></span>|<span data-ttu-id="2c497-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c497-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2c497-156">displayName</span><span class="sxs-lookup"><span data-stu-id="2c497-156">displayName</span></span>|<span data-ttu-id="2c497-157">String</span><span class="sxs-lookup"><span data-stu-id="2c497-157">String</span></span>|<span data-ttu-id="2c497-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="2c497-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2c497-159">version</span><span class="sxs-lookup"><span data-stu-id="2c497-159">version</span></span>|<span data-ttu-id="2c497-160">Int32</span><span class="sxs-lookup"><span data-stu-id="2c497-160">Int32</span></span>|<span data-ttu-id="2c497-161">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2c497-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="2c497-162">响应</span><span class="sxs-lookup"><span data-stu-id="2c497-162">Response</span></span>
<span data-ttu-id="2c497-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c497-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c497-164">示例</span><span class="sxs-lookup"><span data-stu-id="2c497-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c497-165">请求</span><span class="sxs-lookup"><span data-stu-id="2c497-165">Request</span></span>
<span data-ttu-id="2c497-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c497-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c497-167">响应</span><span class="sxs-lookup"><span data-stu-id="2c497-167">Response</span></span>
<span data-ttu-id="2c497-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c497-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





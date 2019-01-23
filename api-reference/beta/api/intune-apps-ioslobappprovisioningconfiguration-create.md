---
title: 创建 iosLobAppProvisioningConfiguration
description: 创建新的 iosLobAppProvisioningConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9821b36ef52080f752adf89be1b6959e6c920b25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405441"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c5ff3-103">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5ff3-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="c5ff3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5ff3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5ff3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5ff3-107">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5ff3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5ff3-108">Prerequisites</span></span>
<span data-ttu-id="c5ff3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5ff3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5ff3-111">Permission type</span></span>|<span data-ttu-id="c5ff3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5ff3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5ff3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5ff3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5ff3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5ff3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5ff3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5ff3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5ff3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-116">Not supported.</span></span>|
|<span data-ttu-id="c5ff3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5ff3-117">Application</span></span>|<span data-ttu-id="c5ff3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5ff3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5ff3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5ff3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5ff3-120">Request headers</span></span>
|<span data-ttu-id="c5ff3-121">标头</span><span class="sxs-lookup"><span data-stu-id="c5ff3-121">Header</span></span>|<span data-ttu-id="c5ff3-122">值</span><span class="sxs-lookup"><span data-stu-id="c5ff3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5ff3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5ff3-123">Authorization</span></span>|<span data-ttu-id="c5ff3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5ff3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5ff3-125">Accept</span></span>|<span data-ttu-id="c5ff3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5ff3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5ff3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5ff3-127">Request body</span></span>
<span data-ttu-id="c5ff3-128">在请求正文中，提供 iosLobAppProvisioningConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="c5ff3-129">下表显示时创建 iosLobAppProvisioningConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="c5ff3-130">属性</span><span class="sxs-lookup"><span data-stu-id="c5ff3-130">Property</span></span>|<span data-ttu-id="c5ff3-131">类型</span><span class="sxs-lookup"><span data-stu-id="c5ff3-131">Type</span></span>|<span data-ttu-id="c5ff3-132">说明</span><span class="sxs-lookup"><span data-stu-id="c5ff3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ff3-133">id</span><span class="sxs-lookup"><span data-stu-id="c5ff3-133">id</span></span>|<span data-ttu-id="c5ff3-134">String</span><span class="sxs-lookup"><span data-stu-id="c5ff3-134">String</span></span>|<span data-ttu-id="c5ff3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-135">Key of the entity.</span></span>|
|<span data-ttu-id="c5ff3-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ff3-136">expirationDateTime</span></span>|<span data-ttu-id="c5ff3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ff3-137">DateTimeOffset</span></span>|<span data-ttu-id="c5ff3-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="c5ff3-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c5ff3-139">payloadFileName</span></span>|<span data-ttu-id="c5ff3-140">String</span><span class="sxs-lookup"><span data-stu-id="c5ff3-140">String</span></span>|<span data-ttu-id="c5ff3-141">负载文件名 (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="c5ff3-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="c5ff3-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-142">\*.xml).</span></span>|
|<span data-ttu-id="c5ff3-143">payload</span><span class="sxs-lookup"><span data-stu-id="c5ff3-143">payload</span></span>|<span data-ttu-id="c5ff3-144">Binary</span><span class="sxs-lookup"><span data-stu-id="c5ff3-144">Binary</span></span>|<span data-ttu-id="c5ff3-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-145">Payload.</span></span> <span data-ttu-id="c5ff3-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="c5ff3-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c5ff3-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ff3-147">createdDateTime</span></span>|<span data-ttu-id="c5ff3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ff3-148">DateTimeOffset</span></span>|<span data-ttu-id="c5ff3-149">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="c5ff3-150">description</span><span class="sxs-lookup"><span data-stu-id="c5ff3-150">description</span></span>|<span data-ttu-id="c5ff3-151">String</span><span class="sxs-lookup"><span data-stu-id="c5ff3-151">String</span></span>|<span data-ttu-id="c5ff3-152">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c5ff3-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ff3-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c5ff3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ff3-154">DateTimeOffset</span></span>|<span data-ttu-id="c5ff3-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c5ff3-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c5ff3-156">displayName</span></span>|<span data-ttu-id="c5ff3-157">String</span><span class="sxs-lookup"><span data-stu-id="c5ff3-157">String</span></span>|<span data-ttu-id="c5ff3-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c5ff3-159">version</span><span class="sxs-lookup"><span data-stu-id="c5ff3-159">version</span></span>|<span data-ttu-id="c5ff3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="c5ff3-160">Int32</span></span>|<span data-ttu-id="c5ff3-161">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c5ff3-162">响应</span><span class="sxs-lookup"><span data-stu-id="c5ff3-162">Response</span></span>
<span data-ttu-id="c5ff3-163">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-163">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5ff3-164">示例</span><span class="sxs-lookup"><span data-stu-id="c5ff3-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5ff3-165">请求</span><span class="sxs-lookup"><span data-stu-id="c5ff3-165">Request</span></span>
<span data-ttu-id="c5ff3-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
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

### <a name="response"></a><span data-ttu-id="c5ff3-167">响应</span><span class="sxs-lookup"><span data-stu-id="c5ff3-167">Response</span></span>
<span data-ttu-id="c5ff3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5ff3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





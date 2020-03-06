---
title: 创建 windowsPhone81CustomConfiguration
description: 创建新的 windowsPhone81CustomConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04ba57de6e80cbc5412a427f351ca23c998e560e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513764"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="fd02d-103">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd02d-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="fd02d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd02d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd02d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd02d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd02d-106">创建新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd02d-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd02d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd02d-107">Prerequisites</span></span>
<span data-ttu-id="fd02d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd02d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd02d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd02d-110">Permission type</span></span>|<span data-ttu-id="fd02d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd02d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd02d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd02d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd02d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd02d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd02d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd02d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd02d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd02d-115">Not supported.</span></span>|
|<span data-ttu-id="fd02d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd02d-116">Application</span></span>|<span data-ttu-id="fd02d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd02d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd02d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd02d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fd02d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd02d-119">Request headers</span></span>
|<span data-ttu-id="fd02d-120">标头</span><span class="sxs-lookup"><span data-stu-id="fd02d-120">Header</span></span>|<span data-ttu-id="fd02d-121">值</span><span class="sxs-lookup"><span data-stu-id="fd02d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd02d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd02d-122">Authorization</span></span>|<span data-ttu-id="fd02d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd02d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd02d-124">接受</span><span class="sxs-lookup"><span data-stu-id="fd02d-124">Accept</span></span>|<span data-ttu-id="fd02d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd02d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd02d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd02d-126">Request body</span></span>
<span data-ttu-id="fd02d-127">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd02d-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="fd02d-128">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd02d-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="fd02d-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd02d-129">Property</span></span>|<span data-ttu-id="fd02d-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd02d-130">Type</span></span>|<span data-ttu-id="fd02d-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd02d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd02d-132">id</span><span class="sxs-lookup"><span data-stu-id="fd02d-132">id</span></span>|<span data-ttu-id="fd02d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fd02d-133">String</span></span>|<span data-ttu-id="fd02d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd02d-134">Key of the entity.</span></span> <span data-ttu-id="fd02d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd02d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fd02d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd02d-137">DateTimeOffset</span></span>|<span data-ttu-id="fd02d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd02d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fd02d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd02d-140">createdDateTime</span></span>|<span data-ttu-id="fd02d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd02d-141">DateTimeOffset</span></span>|<span data-ttu-id="fd02d-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd02d-142">DateTime the object was created.</span></span> <span data-ttu-id="fd02d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-144">说明</span><span class="sxs-lookup"><span data-stu-id="fd02d-144">description</span></span>|<span data-ttu-id="fd02d-145">String</span><span class="sxs-lookup"><span data-stu-id="fd02d-145">String</span></span>|<span data-ttu-id="fd02d-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fd02d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fd02d-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="fd02d-148">displayName</span></span>|<span data-ttu-id="fd02d-149">String</span><span class="sxs-lookup"><span data-stu-id="fd02d-149">String</span></span>|<span data-ttu-id="fd02d-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fd02d-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fd02d-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-152">version</span><span class="sxs-lookup"><span data-stu-id="fd02d-152">version</span></span>|<span data-ttu-id="fd02d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fd02d-153">Int32</span></span>|<span data-ttu-id="fd02d-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fd02d-154">Version of the device configuration.</span></span> <span data-ttu-id="fd02d-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd02d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd02d-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="fd02d-156">omaSettings</span></span>|<span data-ttu-id="fd02d-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd02d-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="fd02d-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="fd02d-158">OMA settings.</span></span> <span data-ttu-id="fd02d-159">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="fd02d-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fd02d-160">响应</span><span class="sxs-lookup"><span data-stu-id="fd02d-160">Response</span></span>
<span data-ttu-id="fd02d-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd02d-161">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd02d-162">示例</span><span class="sxs-lookup"><span data-stu-id="fd02d-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd02d-163">请求</span><span class="sxs-lookup"><span data-stu-id="fd02d-163">Request</span></span>
<span data-ttu-id="fd02d-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd02d-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fd02d-165">响应</span><span class="sxs-lookup"><span data-stu-id="fd02d-165">Response</span></span>
<span data-ttu-id="fd02d-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd02d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```





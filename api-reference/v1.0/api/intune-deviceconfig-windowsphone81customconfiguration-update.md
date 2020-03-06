---
title: 更新 windowsPhone81CustomConfiguration
description: 更新 windowsPhone81CustomConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33d658d6173752befba97452a0eb1d7e9ce960d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513736"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="5da96-103">更新 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5da96-103">Update windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="5da96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5da96-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5da96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5da96-106">更新 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5da96-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5da96-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5da96-107">Prerequisites</span></span>
<span data-ttu-id="5da96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5da96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5da96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5da96-110">Permission type</span></span>|<span data-ttu-id="5da96-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5da96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5da96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5da96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5da96-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da96-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5da96-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5da96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5da96-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5da96-115">Not supported.</span></span>|
|<span data-ttu-id="5da96-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5da96-116">Application</span></span>|<span data-ttu-id="5da96-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5da96-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5da96-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5da96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5da96-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5da96-119">Request headers</span></span>
|<span data-ttu-id="5da96-120">标头</span><span class="sxs-lookup"><span data-stu-id="5da96-120">Header</span></span>|<span data-ttu-id="5da96-121">值</span><span class="sxs-lookup"><span data-stu-id="5da96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5da96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5da96-122">Authorization</span></span>|<span data-ttu-id="5da96-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5da96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5da96-124">接受</span><span class="sxs-lookup"><span data-stu-id="5da96-124">Accept</span></span>|<span data-ttu-id="5da96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5da96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5da96-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5da96-126">Request body</span></span>
<span data-ttu-id="5da96-127">在请求正文中，提供 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5da96-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="5da96-128">下表显示了创建 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5da96-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="5da96-129">属性</span><span class="sxs-lookup"><span data-stu-id="5da96-129">Property</span></span>|<span data-ttu-id="5da96-130">类型</span><span class="sxs-lookup"><span data-stu-id="5da96-130">Type</span></span>|<span data-ttu-id="5da96-131">说明</span><span class="sxs-lookup"><span data-stu-id="5da96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5da96-132">id</span><span class="sxs-lookup"><span data-stu-id="5da96-132">id</span></span>|<span data-ttu-id="5da96-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5da96-133">String</span></span>|<span data-ttu-id="5da96-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5da96-134">Key of the entity.</span></span> <span data-ttu-id="5da96-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5da96-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5da96-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5da96-137">DateTimeOffset</span></span>|<span data-ttu-id="5da96-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5da96-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5da96-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5da96-140">createdDateTime</span></span>|<span data-ttu-id="5da96-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5da96-141">DateTimeOffset</span></span>|<span data-ttu-id="5da96-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5da96-142">DateTime the object was created.</span></span> <span data-ttu-id="5da96-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-144">说明</span><span class="sxs-lookup"><span data-stu-id="5da96-144">description</span></span>|<span data-ttu-id="5da96-145">String</span><span class="sxs-lookup"><span data-stu-id="5da96-145">String</span></span>|<span data-ttu-id="5da96-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5da96-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5da96-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5da96-148">displayName</span></span>|<span data-ttu-id="5da96-149">String</span><span class="sxs-lookup"><span data-stu-id="5da96-149">String</span></span>|<span data-ttu-id="5da96-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5da96-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5da96-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-152">version</span><span class="sxs-lookup"><span data-stu-id="5da96-152">version</span></span>|<span data-ttu-id="5da96-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5da96-153">Int32</span></span>|<span data-ttu-id="5da96-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5da96-154">Version of the device configuration.</span></span> <span data-ttu-id="5da96-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5da96-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5da96-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="5da96-156">omaSettings</span></span>|<span data-ttu-id="5da96-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5da96-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="5da96-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="5da96-158">OMA settings.</span></span> <span data-ttu-id="5da96-159">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="5da96-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5da96-160">响应</span><span class="sxs-lookup"><span data-stu-id="5da96-160">Response</span></span>
<span data-ttu-id="5da96-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5da96-161">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5da96-162">示例</span><span class="sxs-lookup"><span data-stu-id="5da96-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="5da96-163">请求</span><span class="sxs-lookup"><span data-stu-id="5da96-163">Request</span></span>
<span data-ttu-id="5da96-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5da96-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="5da96-165">响应</span><span class="sxs-lookup"><span data-stu-id="5da96-165">Response</span></span>
<span data-ttu-id="5da96-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5da96-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





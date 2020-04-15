---
title: 更新 windowsPhone81CustomConfiguration
description: 更新 windowsPhone81CustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d54e5956f1047f8793bd82ad3eb3302381f1514c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421984"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="ddecf-103">更新 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddecf-103">Update windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="ddecf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddecf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddecf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddecf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddecf-106">更新 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ddecf-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddecf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddecf-107">Prerequisites</span></span>
<span data-ttu-id="ddecf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddecf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddecf-110">Permission type</span></span>|<span data-ttu-id="ddecf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddecf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddecf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddecf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddecf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddecf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddecf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddecf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddecf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddecf-115">Not supported.</span></span>|
|<span data-ttu-id="ddecf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddecf-116">Application</span></span>|<span data-ttu-id="ddecf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddecf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddecf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddecf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ddecf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddecf-119">Request headers</span></span>
|<span data-ttu-id="ddecf-120">标头</span><span class="sxs-lookup"><span data-stu-id="ddecf-120">Header</span></span>|<span data-ttu-id="ddecf-121">值</span><span class="sxs-lookup"><span data-stu-id="ddecf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddecf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddecf-122">Authorization</span></span>|<span data-ttu-id="ddecf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddecf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddecf-124">接受</span><span class="sxs-lookup"><span data-stu-id="ddecf-124">Accept</span></span>|<span data-ttu-id="ddecf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddecf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddecf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddecf-126">Request body</span></span>
<span data-ttu-id="ddecf-127">在请求正文中，提供 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddecf-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="ddecf-128">下表显示了创建 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddecf-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="ddecf-129">属性</span><span class="sxs-lookup"><span data-stu-id="ddecf-129">Property</span></span>|<span data-ttu-id="ddecf-130">类型</span><span class="sxs-lookup"><span data-stu-id="ddecf-130">Type</span></span>|<span data-ttu-id="ddecf-131">说明</span><span class="sxs-lookup"><span data-stu-id="ddecf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddecf-132">id</span><span class="sxs-lookup"><span data-stu-id="ddecf-132">id</span></span>|<span data-ttu-id="ddecf-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ddecf-133">String</span></span>|<span data-ttu-id="ddecf-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddecf-134">Key of the entity.</span></span> <span data-ttu-id="ddecf-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddecf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ddecf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddecf-137">DateTimeOffset</span></span>|<span data-ttu-id="ddecf-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddecf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ddecf-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddecf-140">createdDateTime</span></span>|<span data-ttu-id="ddecf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddecf-141">DateTimeOffset</span></span>|<span data-ttu-id="ddecf-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddecf-142">DateTime the object was created.</span></span> <span data-ttu-id="ddecf-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-144">description</span><span class="sxs-lookup"><span data-stu-id="ddecf-144">description</span></span>|<span data-ttu-id="ddecf-145">String</span><span class="sxs-lookup"><span data-stu-id="ddecf-145">String</span></span>|<span data-ttu-id="ddecf-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddecf-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddecf-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ddecf-148">displayName</span></span>|<span data-ttu-id="ddecf-149">String</span><span class="sxs-lookup"><span data-stu-id="ddecf-149">String</span></span>|<span data-ttu-id="ddecf-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddecf-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddecf-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-152">version</span><span class="sxs-lookup"><span data-stu-id="ddecf-152">version</span></span>|<span data-ttu-id="ddecf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ddecf-153">Int32</span></span>|<span data-ttu-id="ddecf-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddecf-154">Version of the device configuration.</span></span> <span data-ttu-id="ddecf-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddecf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddecf-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ddecf-156">omaSettings</span></span>|<span data-ttu-id="ddecf-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddecf-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ddecf-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="ddecf-158">OMA settings.</span></span> <span data-ttu-id="ddecf-159">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddecf-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ddecf-160">响应</span><span class="sxs-lookup"><span data-stu-id="ddecf-160">Response</span></span>
<span data-ttu-id="ddecf-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddecf-161">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddecf-162">示例</span><span class="sxs-lookup"><span data-stu-id="ddecf-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddecf-163">请求</span><span class="sxs-lookup"><span data-stu-id="ddecf-163">Request</span></span>
<span data-ttu-id="ddecf-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddecf-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddecf-165">响应</span><span class="sxs-lookup"><span data-stu-id="ddecf-165">Response</span></span>
<span data-ttu-id="ddecf-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddecf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







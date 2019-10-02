---
title: 更新 windows10CustomConfiguration
description: 更新 windows10CustomConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4067e25b8a97fbc57a5168c16ded515e9a6092e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365563"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="2065d-103">更新 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2065d-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="2065d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2065d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2065d-105">更新 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2065d-105">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2065d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2065d-106">Prerequisites</span></span>
<span data-ttu-id="2065d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2065d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2065d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2065d-109">Permission type</span></span>|<span data-ttu-id="2065d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2065d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2065d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2065d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2065d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2065d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2065d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2065d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2065d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2065d-114">Not supported.</span></span>|
|<span data-ttu-id="2065d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2065d-115">Application</span></span>|<span data-ttu-id="2065d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2065d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2065d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2065d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2065d-118">请求头</span><span class="sxs-lookup"><span data-stu-id="2065d-118">Request headers</span></span>
|<span data-ttu-id="2065d-119">标头</span><span class="sxs-lookup"><span data-stu-id="2065d-119">Header</span></span>|<span data-ttu-id="2065d-120">值</span><span class="sxs-lookup"><span data-stu-id="2065d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2065d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2065d-121">Authorization</span></span>|<span data-ttu-id="2065d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2065d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2065d-123">接受</span><span class="sxs-lookup"><span data-stu-id="2065d-123">Accept</span></span>|<span data-ttu-id="2065d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2065d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2065d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2065d-125">Request body</span></span>
<span data-ttu-id="2065d-126">在请求正文中，提供 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2065d-126">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="2065d-127">下表显示了创建 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2065d-127">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="2065d-128">属性</span><span class="sxs-lookup"><span data-stu-id="2065d-128">Property</span></span>|<span data-ttu-id="2065d-129">类型</span><span class="sxs-lookup"><span data-stu-id="2065d-129">Type</span></span>|<span data-ttu-id="2065d-130">说明</span><span class="sxs-lookup"><span data-stu-id="2065d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2065d-131">id</span><span class="sxs-lookup"><span data-stu-id="2065d-131">id</span></span>|<span data-ttu-id="2065d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2065d-132">String</span></span>|<span data-ttu-id="2065d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2065d-133">Key of the entity.</span></span> <span data-ttu-id="2065d-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2065d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2065d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2065d-136">DateTimeOffset</span></span>|<span data-ttu-id="2065d-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2065d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2065d-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2065d-139">createdDateTime</span></span>|<span data-ttu-id="2065d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2065d-140">DateTimeOffset</span></span>|<span data-ttu-id="2065d-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2065d-141">DateTime the object was created.</span></span> <span data-ttu-id="2065d-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-143">说明</span><span class="sxs-lookup"><span data-stu-id="2065d-143">description</span></span>|<span data-ttu-id="2065d-144">String</span><span class="sxs-lookup"><span data-stu-id="2065d-144">String</span></span>|<span data-ttu-id="2065d-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2065d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2065d-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2065d-147">displayName</span></span>|<span data-ttu-id="2065d-148">String</span><span class="sxs-lookup"><span data-stu-id="2065d-148">String</span></span>|<span data-ttu-id="2065d-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2065d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2065d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-151">version</span><span class="sxs-lookup"><span data-stu-id="2065d-151">version</span></span>|<span data-ttu-id="2065d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2065d-152">Int32</span></span>|<span data-ttu-id="2065d-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2065d-153">Version of the device configuration.</span></span> <span data-ttu-id="2065d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2065d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2065d-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="2065d-155">omaSettings</span></span>|<span data-ttu-id="2065d-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2065d-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="2065d-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="2065d-157">OMA settings.</span></span> <span data-ttu-id="2065d-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="2065d-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2065d-159">响应</span><span class="sxs-lookup"><span data-stu-id="2065d-159">Response</span></span>
<span data-ttu-id="2065d-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2065d-160">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2065d-161">示例</span><span class="sxs-lookup"><span data-stu-id="2065d-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2065d-162">请求</span><span class="sxs-lookup"><span data-stu-id="2065d-162">Request</span></span>
<span data-ttu-id="2065d-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2065d-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="2065d-164">响应</span><span class="sxs-lookup"><span data-stu-id="2065d-164">Response</span></span>
<span data-ttu-id="2065d-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2065d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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





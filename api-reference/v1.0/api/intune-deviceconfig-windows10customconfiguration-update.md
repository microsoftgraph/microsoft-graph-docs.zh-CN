---
title: 更新 windows10CustomConfiguration
description: 更新 windows10CustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16126906fa4a4127298de60760bf76c0be982310
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758293"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="da123-103">更新 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="da123-103">Update windows10CustomConfiguration</span></span>

<span data-ttu-id="da123-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da123-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da123-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da123-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da123-106">更新 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da123-106">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da123-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da123-107">Prerequisites</span></span>
<span data-ttu-id="da123-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da123-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da123-110">Permission type</span></span>|<span data-ttu-id="da123-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da123-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da123-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da123-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da123-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da123-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da123-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da123-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da123-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da123-115">Not supported.</span></span>|
|<span data-ttu-id="da123-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da123-116">Application</span></span>|<span data-ttu-id="da123-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da123-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da123-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da123-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da123-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da123-119">Request headers</span></span>
|<span data-ttu-id="da123-120">标头</span><span class="sxs-lookup"><span data-stu-id="da123-120">Header</span></span>|<span data-ttu-id="da123-121">值</span><span class="sxs-lookup"><span data-stu-id="da123-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da123-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da123-122">Authorization</span></span>|<span data-ttu-id="da123-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da123-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da123-124">接受</span><span class="sxs-lookup"><span data-stu-id="da123-124">Accept</span></span>|<span data-ttu-id="da123-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da123-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da123-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da123-126">Request body</span></span>
<span data-ttu-id="da123-127">在请求正文中，提供 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da123-127">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="da123-128">下表显示了创建 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da123-128">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="da123-129">属性</span><span class="sxs-lookup"><span data-stu-id="da123-129">Property</span></span>|<span data-ttu-id="da123-130">类型</span><span class="sxs-lookup"><span data-stu-id="da123-130">Type</span></span>|<span data-ttu-id="da123-131">说明</span><span class="sxs-lookup"><span data-stu-id="da123-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da123-132">id</span><span class="sxs-lookup"><span data-stu-id="da123-132">id</span></span>|<span data-ttu-id="da123-133">String</span><span class="sxs-lookup"><span data-stu-id="da123-133">String</span></span>|<span data-ttu-id="da123-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da123-134">Key of the entity.</span></span> <span data-ttu-id="da123-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da123-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da123-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da123-137">DateTimeOffset</span></span>|<span data-ttu-id="da123-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da123-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da123-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da123-140">createdDateTime</span></span>|<span data-ttu-id="da123-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da123-141">DateTimeOffset</span></span>|<span data-ttu-id="da123-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da123-142">DateTime the object was created.</span></span> <span data-ttu-id="da123-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-144">description</span><span class="sxs-lookup"><span data-stu-id="da123-144">description</span></span>|<span data-ttu-id="da123-145">String</span><span class="sxs-lookup"><span data-stu-id="da123-145">String</span></span>|<span data-ttu-id="da123-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="da123-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da123-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-148">displayName</span><span class="sxs-lookup"><span data-stu-id="da123-148">displayName</span></span>|<span data-ttu-id="da123-149">String</span><span class="sxs-lookup"><span data-stu-id="da123-149">String</span></span>|<span data-ttu-id="da123-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="da123-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da123-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-152">version</span><span class="sxs-lookup"><span data-stu-id="da123-152">version</span></span>|<span data-ttu-id="da123-153">Int32</span><span class="sxs-lookup"><span data-stu-id="da123-153">Int32</span></span>|<span data-ttu-id="da123-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="da123-154">Version of the device configuration.</span></span> <span data-ttu-id="da123-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da123-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da123-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="da123-156">omaSettings</span></span>|<span data-ttu-id="da123-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da123-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="da123-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="da123-158">OMA settings.</span></span> <span data-ttu-id="da123-159">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="da123-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="da123-160">响应</span><span class="sxs-lookup"><span data-stu-id="da123-160">Response</span></span>
<span data-ttu-id="da123-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da123-161">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da123-162">示例</span><span class="sxs-lookup"><span data-stu-id="da123-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="da123-163">请求</span><span class="sxs-lookup"><span data-stu-id="da123-163">Request</span></span>
<span data-ttu-id="da123-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da123-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="da123-165">响应</span><span class="sxs-lookup"><span data-stu-id="da123-165">Response</span></span>
<span data-ttu-id="da123-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da123-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```





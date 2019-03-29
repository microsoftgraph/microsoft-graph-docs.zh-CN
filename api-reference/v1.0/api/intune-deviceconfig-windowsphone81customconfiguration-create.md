---
title: 创建 windowsPhone81CustomConfiguration
description: 创建新的 windowsPhone81CustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b04ad9901263d0e9815011f0c8b067e6520ed89b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968047"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="1016f-103">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1016f-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="1016f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1016f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1016f-105">创建新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1016f-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1016f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1016f-106">Prerequisites</span></span>
<span data-ttu-id="1016f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1016f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1016f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1016f-109">Permission type</span></span>|<span data-ttu-id="1016f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1016f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1016f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1016f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1016f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1016f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1016f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1016f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1016f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1016f-114">Not supported.</span></span>|
|<span data-ttu-id="1016f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1016f-115">Application</span></span>|<span data-ttu-id="1016f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1016f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1016f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1016f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1016f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1016f-118">Request headers</span></span>
|<span data-ttu-id="1016f-119">标头</span><span class="sxs-lookup"><span data-stu-id="1016f-119">Header</span></span>|<span data-ttu-id="1016f-120">值</span><span class="sxs-lookup"><span data-stu-id="1016f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1016f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1016f-121">Authorization</span></span>|<span data-ttu-id="1016f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1016f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1016f-123">接受</span><span class="sxs-lookup"><span data-stu-id="1016f-123">Accept</span></span>|<span data-ttu-id="1016f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1016f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1016f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1016f-125">Request body</span></span>
<span data-ttu-id="1016f-126">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1016f-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="1016f-127">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1016f-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="1016f-128">属性</span><span class="sxs-lookup"><span data-stu-id="1016f-128">Property</span></span>|<span data-ttu-id="1016f-129">类型</span><span class="sxs-lookup"><span data-stu-id="1016f-129">Type</span></span>|<span data-ttu-id="1016f-130">说明</span><span class="sxs-lookup"><span data-stu-id="1016f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1016f-131">id</span><span class="sxs-lookup"><span data-stu-id="1016f-131">id</span></span>|<span data-ttu-id="1016f-132">String</span><span class="sxs-lookup"><span data-stu-id="1016f-132">String</span></span>|<span data-ttu-id="1016f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1016f-133">Key of the entity.</span></span> <span data-ttu-id="1016f-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1016f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1016f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1016f-136">DateTimeOffset</span></span>|<span data-ttu-id="1016f-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1016f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1016f-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1016f-139">createdDateTime</span></span>|<span data-ttu-id="1016f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1016f-140">DateTimeOffset</span></span>|<span data-ttu-id="1016f-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1016f-141">DateTime the object was created.</span></span> <span data-ttu-id="1016f-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-143">description</span><span class="sxs-lookup"><span data-stu-id="1016f-143">description</span></span>|<span data-ttu-id="1016f-144">String</span><span class="sxs-lookup"><span data-stu-id="1016f-144">String</span></span>|<span data-ttu-id="1016f-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1016f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1016f-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1016f-147">displayName</span></span>|<span data-ttu-id="1016f-148">String</span><span class="sxs-lookup"><span data-stu-id="1016f-148">String</span></span>|<span data-ttu-id="1016f-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1016f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1016f-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-151">version</span><span class="sxs-lookup"><span data-stu-id="1016f-151">version</span></span>|<span data-ttu-id="1016f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1016f-152">Int32</span></span>|<span data-ttu-id="1016f-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1016f-153">Version of the device configuration.</span></span> <span data-ttu-id="1016f-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1016f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1016f-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1016f-155">omaSettings</span></span>|<span data-ttu-id="1016f-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1016f-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="1016f-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="1016f-157">OMA settings.</span></span> <span data-ttu-id="1016f-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="1016f-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1016f-159">响应</span><span class="sxs-lookup"><span data-stu-id="1016f-159">Response</span></span>
<span data-ttu-id="1016f-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1016f-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1016f-161">示例</span><span class="sxs-lookup"><span data-stu-id="1016f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="1016f-162">请求</span><span class="sxs-lookup"><span data-stu-id="1016f-162">Request</span></span>
<span data-ttu-id="1016f-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1016f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1016f-164">响应</span><span class="sxs-lookup"><span data-stu-id="1016f-164">Response</span></span>
<span data-ttu-id="1016f-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1016f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




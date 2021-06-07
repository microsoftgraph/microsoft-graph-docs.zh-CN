---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 540c30178ff06b5520042213d4a80396de6ed963
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759161"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="20b6e-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="20b6e-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="20b6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20b6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20b6e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20b6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b6e-106">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20b6e-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20b6e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="20b6e-107">Prerequisites</span></span>
<span data-ttu-id="20b6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b6e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="20b6e-110">Permission type</span></span>|<span data-ttu-id="20b6e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20b6e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20b6e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20b6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20b6e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20b6e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20b6e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20b6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20b6e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="20b6e-115">Not supported.</span></span>|
|<span data-ttu-id="20b6e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="20b6e-116">Application</span></span>|<span data-ttu-id="20b6e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20b6e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20b6e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20b6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="20b6e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="20b6e-119">Request headers</span></span>
|<span data-ttu-id="20b6e-120">标头</span><span class="sxs-lookup"><span data-stu-id="20b6e-120">Header</span></span>|<span data-ttu-id="20b6e-121">值</span><span class="sxs-lookup"><span data-stu-id="20b6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b6e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20b6e-122">Authorization</span></span>|<span data-ttu-id="20b6e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20b6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b6e-124">接受</span><span class="sxs-lookup"><span data-stu-id="20b6e-124">Accept</span></span>|<span data-ttu-id="20b6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20b6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b6e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="20b6e-126">Request body</span></span>
<span data-ttu-id="20b6e-127">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20b6e-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="20b6e-128">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20b6e-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="20b6e-129">属性</span><span class="sxs-lookup"><span data-stu-id="20b6e-129">Property</span></span>|<span data-ttu-id="20b6e-130">类型</span><span class="sxs-lookup"><span data-stu-id="20b6e-130">Type</span></span>|<span data-ttu-id="20b6e-131">说明</span><span class="sxs-lookup"><span data-stu-id="20b6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b6e-132">id</span><span class="sxs-lookup"><span data-stu-id="20b6e-132">id</span></span>|<span data-ttu-id="20b6e-133">String</span><span class="sxs-lookup"><span data-stu-id="20b6e-133">String</span></span>|<span data-ttu-id="20b6e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="20b6e-134">Key of the entity.</span></span> <span data-ttu-id="20b6e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20b6e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="20b6e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b6e-137">DateTimeOffset</span></span>|<span data-ttu-id="20b6e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="20b6e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="20b6e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20b6e-140">createdDateTime</span></span>|<span data-ttu-id="20b6e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b6e-141">DateTimeOffset</span></span>|<span data-ttu-id="20b6e-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="20b6e-142">DateTime the object was created.</span></span> <span data-ttu-id="20b6e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-144">description</span><span class="sxs-lookup"><span data-stu-id="20b6e-144">description</span></span>|<span data-ttu-id="20b6e-145">String</span><span class="sxs-lookup"><span data-stu-id="20b6e-145">String</span></span>|<span data-ttu-id="20b6e-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="20b6e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20b6e-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="20b6e-148">displayName</span></span>|<span data-ttu-id="20b6e-149">String</span><span class="sxs-lookup"><span data-stu-id="20b6e-149">String</span></span>|<span data-ttu-id="20b6e-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="20b6e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20b6e-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-152">version</span><span class="sxs-lookup"><span data-stu-id="20b6e-152">version</span></span>|<span data-ttu-id="20b6e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="20b6e-153">Int32</span></span>|<span data-ttu-id="20b6e-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="20b6e-154">Version of the device configuration.</span></span> <span data-ttu-id="20b6e-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20b6e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6e-156">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="20b6e-156">allowSampleSharing</span></span>|<span data-ttu-id="20b6e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="20b6e-157">Boolean</span></span>|<span data-ttu-id="20b6e-158">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="20b6e-158">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="20b6e-159">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="20b6e-159">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="20b6e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="20b6e-160">Boolean</span></span>|<span data-ttu-id="20b6e-161">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="20b6e-161">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="20b6e-162">响应</span><span class="sxs-lookup"><span data-stu-id="20b6e-162">Response</span></span>
<span data-ttu-id="20b6e-163">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20b6e-163">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b6e-164">示例</span><span class="sxs-lookup"><span data-stu-id="20b6e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="20b6e-165">请求</span><span class="sxs-lookup"><span data-stu-id="20b6e-165">Request</span></span>
<span data-ttu-id="20b6e-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20b6e-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="20b6e-167">响应</span><span class="sxs-lookup"><span data-stu-id="20b6e-167">Response</span></span>
<span data-ttu-id="20b6e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20b6e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```





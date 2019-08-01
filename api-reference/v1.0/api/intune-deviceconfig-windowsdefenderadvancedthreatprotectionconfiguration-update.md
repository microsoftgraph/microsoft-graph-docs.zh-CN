---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9444397e61ee64a056600b77afac8cf7b1075e3b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997085"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="9b994-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b994-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="9b994-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b994-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b994-105">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b994-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b994-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b994-106">Prerequisites</span></span>
<span data-ttu-id="9b994-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b994-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b994-109">Permission type</span></span>|<span data-ttu-id="9b994-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b994-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b994-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b994-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b994-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b994-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b994-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b994-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b994-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b994-114">Not supported.</span></span>|
|<span data-ttu-id="9b994-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b994-115">Application</span></span>|<span data-ttu-id="9b994-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b994-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b994-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b994-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b994-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b994-118">Request headers</span></span>
|<span data-ttu-id="9b994-119">标头</span><span class="sxs-lookup"><span data-stu-id="9b994-119">Header</span></span>|<span data-ttu-id="9b994-120">值</span><span class="sxs-lookup"><span data-stu-id="9b994-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b994-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b994-121">Authorization</span></span>|<span data-ttu-id="9b994-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b994-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b994-123">接受</span><span class="sxs-lookup"><span data-stu-id="9b994-123">Accept</span></span>|<span data-ttu-id="9b994-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b994-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b994-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b994-125">Request body</span></span>
<span data-ttu-id="9b994-126">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b994-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="9b994-127">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b994-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="9b994-128">属性</span><span class="sxs-lookup"><span data-stu-id="9b994-128">Property</span></span>|<span data-ttu-id="9b994-129">类型</span><span class="sxs-lookup"><span data-stu-id="9b994-129">Type</span></span>|<span data-ttu-id="9b994-130">说明</span><span class="sxs-lookup"><span data-stu-id="9b994-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b994-131">id</span><span class="sxs-lookup"><span data-stu-id="9b994-131">id</span></span>|<span data-ttu-id="9b994-132">字符串</span><span class="sxs-lookup"><span data-stu-id="9b994-132">String</span></span>|<span data-ttu-id="9b994-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b994-133">Key of the entity.</span></span> <span data-ttu-id="9b994-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b994-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9b994-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b994-136">DateTimeOffset</span></span>|<span data-ttu-id="9b994-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b994-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9b994-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b994-139">createdDateTime</span></span>|<span data-ttu-id="9b994-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b994-140">DateTimeOffset</span></span>|<span data-ttu-id="9b994-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b994-141">DateTime the object was created.</span></span> <span data-ttu-id="9b994-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-143">说明</span><span class="sxs-lookup"><span data-stu-id="9b994-143">description</span></span>|<span data-ttu-id="9b994-144">String</span><span class="sxs-lookup"><span data-stu-id="9b994-144">String</span></span>|<span data-ttu-id="9b994-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9b994-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b994-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9b994-147">displayName</span></span>|<span data-ttu-id="9b994-148">String</span><span class="sxs-lookup"><span data-stu-id="9b994-148">String</span></span>|<span data-ttu-id="9b994-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9b994-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b994-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-151">version</span><span class="sxs-lookup"><span data-stu-id="9b994-151">version</span></span>|<span data-ttu-id="9b994-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9b994-152">Int32</span></span>|<span data-ttu-id="9b994-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9b994-153">Version of the device configuration.</span></span> <span data-ttu-id="9b994-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b994-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b994-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="9b994-155">allowSampleSharing</span></span>|<span data-ttu-id="9b994-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b994-156">Boolean</span></span>|<span data-ttu-id="9b994-157">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="9b994-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="9b994-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="9b994-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="9b994-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b994-159">Boolean</span></span>|<span data-ttu-id="9b994-160">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="9b994-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="9b994-161">响应</span><span class="sxs-lookup"><span data-stu-id="9b994-161">Response</span></span>
<span data-ttu-id="9b994-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b994-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b994-163">示例</span><span class="sxs-lookup"><span data-stu-id="9b994-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b994-164">请求</span><span class="sxs-lookup"><span data-stu-id="9b994-164">Request</span></span>
<span data-ttu-id="9b994-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b994-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b994-166">响应</span><span class="sxs-lookup"><span data-stu-id="9b994-166">Response</span></span>
<span data-ttu-id="9b994-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b994-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




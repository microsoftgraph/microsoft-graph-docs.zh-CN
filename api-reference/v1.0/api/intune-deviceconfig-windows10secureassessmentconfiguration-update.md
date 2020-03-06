---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afe7ecd5951dc554762762ec9bfdb05b8f8d99cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513949"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="f5aad-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5aad-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="f5aad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5aad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5aad-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5aad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5aad-106">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f5aad-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5aad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5aad-107">Prerequisites</span></span>
<span data-ttu-id="f5aad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5aad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5aad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5aad-110">Permission type</span></span>|<span data-ttu-id="f5aad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5aad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5aad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5aad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5aad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5aad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5aad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5aad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5aad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5aad-115">Not supported.</span></span>|
|<span data-ttu-id="f5aad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5aad-116">Application</span></span>|<span data-ttu-id="f5aad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5aad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5aad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5aad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f5aad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5aad-119">Request headers</span></span>
|<span data-ttu-id="f5aad-120">标头</span><span class="sxs-lookup"><span data-stu-id="f5aad-120">Header</span></span>|<span data-ttu-id="f5aad-121">值</span><span class="sxs-lookup"><span data-stu-id="f5aad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5aad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5aad-122">Authorization</span></span>|<span data-ttu-id="f5aad-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5aad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5aad-124">接受</span><span class="sxs-lookup"><span data-stu-id="f5aad-124">Accept</span></span>|<span data-ttu-id="f5aad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5aad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5aad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5aad-126">Request body</span></span>
<span data-ttu-id="f5aad-127">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5aad-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="f5aad-128">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5aad-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="f5aad-129">属性</span><span class="sxs-lookup"><span data-stu-id="f5aad-129">Property</span></span>|<span data-ttu-id="f5aad-130">类型</span><span class="sxs-lookup"><span data-stu-id="f5aad-130">Type</span></span>|<span data-ttu-id="f5aad-131">说明</span><span class="sxs-lookup"><span data-stu-id="f5aad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5aad-132">id</span><span class="sxs-lookup"><span data-stu-id="f5aad-132">id</span></span>|<span data-ttu-id="f5aad-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f5aad-133">String</span></span>|<span data-ttu-id="f5aad-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5aad-134">Key of the entity.</span></span> <span data-ttu-id="f5aad-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5aad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f5aad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5aad-137">DateTimeOffset</span></span>|<span data-ttu-id="f5aad-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5aad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f5aad-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5aad-140">createdDateTime</span></span>|<span data-ttu-id="f5aad-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5aad-141">DateTimeOffset</span></span>|<span data-ttu-id="f5aad-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5aad-142">DateTime the object was created.</span></span> <span data-ttu-id="f5aad-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-144">说明</span><span class="sxs-lookup"><span data-stu-id="f5aad-144">description</span></span>|<span data-ttu-id="f5aad-145">String</span><span class="sxs-lookup"><span data-stu-id="f5aad-145">String</span></span>|<span data-ttu-id="f5aad-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f5aad-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5aad-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f5aad-148">displayName</span></span>|<span data-ttu-id="f5aad-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f5aad-149">String</span></span>|<span data-ttu-id="f5aad-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f5aad-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5aad-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-152">version</span><span class="sxs-lookup"><span data-stu-id="f5aad-152">version</span></span>|<span data-ttu-id="f5aad-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f5aad-153">Int32</span></span>|<span data-ttu-id="f5aad-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f5aad-154">Version of the device configuration.</span></span> <span data-ttu-id="f5aad-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5aad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5aad-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="f5aad-156">launchUri</span></span>|<span data-ttu-id="f5aad-157">字符串</span><span class="sxs-lookup"><span data-stu-id="f5aad-157">String</span></span>|<span data-ttu-id="f5aad-158">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="f5aad-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="f5aad-159">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="f5aad-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="f5aad-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="f5aad-160">configurationAccount</span></span>|<span data-ttu-id="f5aad-161">String</span><span class="sxs-lookup"><span data-stu-id="f5aad-161">String</span></span>|<span data-ttu-id="f5aad-162">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="f5aad-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="f5aad-163">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="f5aad-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="f5aad-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="f5aad-164">allowPrinting</span></span>|<span data-ttu-id="f5aad-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5aad-165">Boolean</span></span>|<span data-ttu-id="f5aad-166">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="f5aad-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="f5aad-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f5aad-167">allowScreenCapture</span></span>|<span data-ttu-id="f5aad-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5aad-168">Boolean</span></span>|<span data-ttu-id="f5aad-169">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="f5aad-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="f5aad-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="f5aad-170">allowTextSuggestion</span></span>|<span data-ttu-id="f5aad-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5aad-171">Boolean</span></span>|<span data-ttu-id="f5aad-172">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="f5aad-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="f5aad-173">响应</span><span class="sxs-lookup"><span data-stu-id="f5aad-173">Response</span></span>
<span data-ttu-id="f5aad-174">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5aad-174">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5aad-175">示例</span><span class="sxs-lookup"><span data-stu-id="f5aad-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5aad-176">请求</span><span class="sxs-lookup"><span data-stu-id="f5aad-176">Request</span></span>
<span data-ttu-id="f5aad-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5aad-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="f5aad-178">响应</span><span class="sxs-lookup"><span data-stu-id="f5aad-178">Response</span></span>
<span data-ttu-id="f5aad-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5aad-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```





---
title: 创建 windows10SecureAssessmentConfiguration
description: 创建新的 windows10SecureAssessmentConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d19b2659e58c71a95266e2cda9209b7ccfac50a5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760480"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="3c745-103">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c745-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="3c745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c745-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c745-106">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c745-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c745-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c745-107">Prerequisites</span></span>
<span data-ttu-id="3c745-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c745-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c745-110">Permission type</span></span>|<span data-ttu-id="3c745-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c745-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c745-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c745-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c745-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c745-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c745-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c745-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c745-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c745-115">Not supported.</span></span>|
|<span data-ttu-id="3c745-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c745-116">Application</span></span>|<span data-ttu-id="3c745-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c745-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c745-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c745-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c745-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c745-119">Request headers</span></span>
|<span data-ttu-id="3c745-120">标头</span><span class="sxs-lookup"><span data-stu-id="3c745-120">Header</span></span>|<span data-ttu-id="3c745-121">值</span><span class="sxs-lookup"><span data-stu-id="3c745-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c745-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c745-122">Authorization</span></span>|<span data-ttu-id="3c745-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c745-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c745-124">接受</span><span class="sxs-lookup"><span data-stu-id="3c745-124">Accept</span></span>|<span data-ttu-id="3c745-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c745-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c745-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c745-126">Request body</span></span>
<span data-ttu-id="3c745-127">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c745-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="3c745-128">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c745-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="3c745-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c745-129">Property</span></span>|<span data-ttu-id="3c745-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c745-130">Type</span></span>|<span data-ttu-id="3c745-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c745-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c745-132">id</span><span class="sxs-lookup"><span data-stu-id="3c745-132">id</span></span>|<span data-ttu-id="3c745-133">String</span><span class="sxs-lookup"><span data-stu-id="3c745-133">String</span></span>|<span data-ttu-id="3c745-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c745-134">Key of the entity.</span></span> <span data-ttu-id="3c745-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c745-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3c745-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c745-137">DateTimeOffset</span></span>|<span data-ttu-id="3c745-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c745-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3c745-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c745-140">createdDateTime</span></span>|<span data-ttu-id="3c745-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c745-141">DateTimeOffset</span></span>|<span data-ttu-id="3c745-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c745-142">DateTime the object was created.</span></span> <span data-ttu-id="3c745-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-144">description</span><span class="sxs-lookup"><span data-stu-id="3c745-144">description</span></span>|<span data-ttu-id="3c745-145">String</span><span class="sxs-lookup"><span data-stu-id="3c745-145">String</span></span>|<span data-ttu-id="3c745-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3c745-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c745-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3c745-148">displayName</span></span>|<span data-ttu-id="3c745-149">String</span><span class="sxs-lookup"><span data-stu-id="3c745-149">String</span></span>|<span data-ttu-id="3c745-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3c745-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c745-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-152">version</span><span class="sxs-lookup"><span data-stu-id="3c745-152">version</span></span>|<span data-ttu-id="3c745-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3c745-153">Int32</span></span>|<span data-ttu-id="3c745-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3c745-154">Version of the device configuration.</span></span> <span data-ttu-id="3c745-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c745-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c745-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="3c745-156">launchUri</span></span>|<span data-ttu-id="3c745-157">String</span><span class="sxs-lookup"><span data-stu-id="3c745-157">String</span></span>|<span data-ttu-id="3c745-158">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="3c745-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="3c745-159">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="3c745-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="3c745-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="3c745-160">configurationAccount</span></span>|<span data-ttu-id="3c745-161">String</span><span class="sxs-lookup"><span data-stu-id="3c745-161">String</span></span>|<span data-ttu-id="3c745-162">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="3c745-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="3c745-163">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="3c745-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="3c745-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="3c745-164">allowPrinting</span></span>|<span data-ttu-id="3c745-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c745-165">Boolean</span></span>|<span data-ttu-id="3c745-166">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="3c745-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="3c745-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="3c745-167">allowScreenCapture</span></span>|<span data-ttu-id="3c745-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c745-168">Boolean</span></span>|<span data-ttu-id="3c745-169">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="3c745-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="3c745-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="3c745-170">allowTextSuggestion</span></span>|<span data-ttu-id="3c745-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c745-171">Boolean</span></span>|<span data-ttu-id="3c745-172">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="3c745-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="3c745-173">响应</span><span class="sxs-lookup"><span data-stu-id="3c745-173">Response</span></span>
<span data-ttu-id="3c745-174">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c745-174">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c745-175">示例</span><span class="sxs-lookup"><span data-stu-id="3c745-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c745-176">请求</span><span class="sxs-lookup"><span data-stu-id="3c745-176">Request</span></span>
<span data-ttu-id="3c745-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c745-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3c745-178">响应</span><span class="sxs-lookup"><span data-stu-id="3c745-178">Response</span></span>
<span data-ttu-id="3c745-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c745-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





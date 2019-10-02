---
title: 创建 windows10SecureAssessmentConfiguration
description: 创建新的 windows10SecureAssessmentConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2919ce12936e5d7387f857de4e5381196c9b5bb9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365262"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="22f30-103">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="22f30-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="22f30-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22f30-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f30-105">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22f30-105">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f30-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="22f30-106">Prerequisites</span></span>
<span data-ttu-id="22f30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22f30-109">Permission type</span></span>|<span data-ttu-id="22f30-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="22f30-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22f30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22f30-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f30-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22f30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22f30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22f30-114">Not supported.</span></span>|
|<span data-ttu-id="22f30-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22f30-115">Application</span></span>|<span data-ttu-id="22f30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22f30-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22f30-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22f30-118">请求头</span><span class="sxs-lookup"><span data-stu-id="22f30-118">Request headers</span></span>
|<span data-ttu-id="22f30-119">标头</span><span class="sxs-lookup"><span data-stu-id="22f30-119">Header</span></span>|<span data-ttu-id="22f30-120">值</span><span class="sxs-lookup"><span data-stu-id="22f30-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f30-121">Authorization</span></span>|<span data-ttu-id="22f30-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22f30-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f30-123">接受</span><span class="sxs-lookup"><span data-stu-id="22f30-123">Accept</span></span>|<span data-ttu-id="22f30-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22f30-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f30-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="22f30-125">Request body</span></span>
<span data-ttu-id="22f30-126">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22f30-126">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="22f30-127">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="22f30-127">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="22f30-128">属性</span><span class="sxs-lookup"><span data-stu-id="22f30-128">Property</span></span>|<span data-ttu-id="22f30-129">类型</span><span class="sxs-lookup"><span data-stu-id="22f30-129">Type</span></span>|<span data-ttu-id="22f30-130">说明</span><span class="sxs-lookup"><span data-stu-id="22f30-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f30-131">id</span><span class="sxs-lookup"><span data-stu-id="22f30-131">id</span></span>|<span data-ttu-id="22f30-132">字符串</span><span class="sxs-lookup"><span data-stu-id="22f30-132">String</span></span>|<span data-ttu-id="22f30-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="22f30-133">Key of the entity.</span></span> <span data-ttu-id="22f30-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22f30-135">lastModifiedDateTime</span></span>|<span data-ttu-id="22f30-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f30-136">DateTimeOffset</span></span>|<span data-ttu-id="22f30-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22f30-137">DateTime the object was last modified.</span></span> <span data-ttu-id="22f30-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22f30-139">createdDateTime</span></span>|<span data-ttu-id="22f30-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f30-140">DateTimeOffset</span></span>|<span data-ttu-id="22f30-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22f30-141">DateTime the object was created.</span></span> <span data-ttu-id="22f30-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-143">说明</span><span class="sxs-lookup"><span data-stu-id="22f30-143">description</span></span>|<span data-ttu-id="22f30-144">String</span><span class="sxs-lookup"><span data-stu-id="22f30-144">String</span></span>|<span data-ttu-id="22f30-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="22f30-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22f30-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-147">displayName</span><span class="sxs-lookup"><span data-stu-id="22f30-147">displayName</span></span>|<span data-ttu-id="22f30-148">字符串</span><span class="sxs-lookup"><span data-stu-id="22f30-148">String</span></span>|<span data-ttu-id="22f30-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="22f30-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22f30-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-151">version</span><span class="sxs-lookup"><span data-stu-id="22f30-151">version</span></span>|<span data-ttu-id="22f30-152">Int32</span><span class="sxs-lookup"><span data-stu-id="22f30-152">Int32</span></span>|<span data-ttu-id="22f30-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="22f30-153">Version of the device configuration.</span></span> <span data-ttu-id="22f30-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f30-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f30-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="22f30-155">launchUri</span></span>|<span data-ttu-id="22f30-156">String</span><span class="sxs-lookup"><span data-stu-id="22f30-156">String</span></span>|<span data-ttu-id="22f30-157">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="22f30-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="22f30-158">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="22f30-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="22f30-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="22f30-159">configurationAccount</span></span>|<span data-ttu-id="22f30-160">String</span><span class="sxs-lookup"><span data-stu-id="22f30-160">String</span></span>|<span data-ttu-id="22f30-161">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="22f30-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="22f30-162">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="22f30-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="22f30-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="22f30-163">allowPrinting</span></span>|<span data-ttu-id="22f30-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="22f30-164">Boolean</span></span>|<span data-ttu-id="22f30-165">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="22f30-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="22f30-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="22f30-166">allowScreenCapture</span></span>|<span data-ttu-id="22f30-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="22f30-167">Boolean</span></span>|<span data-ttu-id="22f30-168">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="22f30-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="22f30-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="22f30-169">allowTextSuggestion</span></span>|<span data-ttu-id="22f30-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="22f30-170">Boolean</span></span>|<span data-ttu-id="22f30-171">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="22f30-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="22f30-172">响应</span><span class="sxs-lookup"><span data-stu-id="22f30-172">Response</span></span>
<span data-ttu-id="22f30-173">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22f30-173">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f30-174">示例</span><span class="sxs-lookup"><span data-stu-id="22f30-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f30-175">请求</span><span class="sxs-lookup"><span data-stu-id="22f30-175">Request</span></span>
<span data-ttu-id="22f30-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22f30-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22f30-177">响应</span><span class="sxs-lookup"><span data-stu-id="22f30-177">Response</span></span>
<span data-ttu-id="22f30-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22f30-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





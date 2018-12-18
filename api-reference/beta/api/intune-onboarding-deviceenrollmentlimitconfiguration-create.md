---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: fdb9fee09f43890280ef0beb79d6d57d9def67f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359666"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="86c66-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="86c66-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="86c66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="86c66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86c66-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86c66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86c66-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="86c66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86c66-107">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86c66-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86c66-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86c66-108">Prerequisites</span></span>
<span data-ttu-id="86c66-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="86c66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c66-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86c66-111">Permission type</span></span>|<span data-ttu-id="86c66-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86c66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c66-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86c66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86c66-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c66-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86c66-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86c66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c66-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86c66-116">Not supported.</span></span>|
|<span data-ttu-id="86c66-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86c66-117">Application</span></span>|<span data-ttu-id="86c66-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="86c66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c66-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86c66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86c66-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86c66-120">Request headers</span></span>
|<span data-ttu-id="86c66-121">标头</span><span class="sxs-lookup"><span data-stu-id="86c66-121">Header</span></span>|<span data-ttu-id="86c66-122">值</span><span class="sxs-lookup"><span data-stu-id="86c66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c66-123">授权</span><span class="sxs-lookup"><span data-stu-id="86c66-123">Authorization</span></span>|<span data-ttu-id="86c66-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86c66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86c66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86c66-125">Accept</span></span>|<span data-ttu-id="86c66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86c66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86c66-127">Request body</span></span>
<span data-ttu-id="86c66-128">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86c66-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="86c66-129">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86c66-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="86c66-130">属性</span><span class="sxs-lookup"><span data-stu-id="86c66-130">Property</span></span>|<span data-ttu-id="86c66-131">类型</span><span class="sxs-lookup"><span data-stu-id="86c66-131">Type</span></span>|<span data-ttu-id="86c66-132">说明</span><span class="sxs-lookup"><span data-stu-id="86c66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c66-133">id</span><span class="sxs-lookup"><span data-stu-id="86c66-133">id</span></span>|<span data-ttu-id="86c66-134">String</span><span class="sxs-lookup"><span data-stu-id="86c66-134">String</span></span>|<span data-ttu-id="86c66-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-136">displayName</span><span class="sxs-lookup"><span data-stu-id="86c66-136">displayName</span></span>|<span data-ttu-id="86c66-137">String</span><span class="sxs-lookup"><span data-stu-id="86c66-137">String</span></span>|<span data-ttu-id="86c66-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-139">description</span><span class="sxs-lookup"><span data-stu-id="86c66-139">description</span></span>|<span data-ttu-id="86c66-140">String</span><span class="sxs-lookup"><span data-stu-id="86c66-140">String</span></span>|<span data-ttu-id="86c66-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-142">priority</span><span class="sxs-lookup"><span data-stu-id="86c66-142">priority</span></span>|<span data-ttu-id="86c66-143">Int32</span><span class="sxs-lookup"><span data-stu-id="86c66-143">Int32</span></span>|<span data-ttu-id="86c66-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86c66-145">createdDateTime</span></span>|<span data-ttu-id="86c66-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c66-146">DateTimeOffset</span></span>|<span data-ttu-id="86c66-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86c66-148">lastModifiedDateTime</span></span>|<span data-ttu-id="86c66-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c66-149">DateTimeOffset</span></span>|<span data-ttu-id="86c66-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-151">version</span><span class="sxs-lookup"><span data-stu-id="86c66-151">version</span></span>|<span data-ttu-id="86c66-152">Int32</span><span class="sxs-lookup"><span data-stu-id="86c66-152">Int32</span></span>|<span data-ttu-id="86c66-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86c66-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86c66-154">limit</span><span class="sxs-lookup"><span data-stu-id="86c66-154">limit</span></span>|<span data-ttu-id="86c66-155">Int32</span><span class="sxs-lookup"><span data-stu-id="86c66-155">Int32</span></span>|<span data-ttu-id="86c66-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86c66-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86c66-157">响应</span><span class="sxs-lookup"><span data-stu-id="86c66-157">Response</span></span>
<span data-ttu-id="86c66-158">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86c66-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c66-159">示例</span><span class="sxs-lookup"><span data-stu-id="86c66-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="86c66-160">请求</span><span class="sxs-lookup"><span data-stu-id="86c66-160">Request</span></span>
<span data-ttu-id="86c66-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86c66-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="86c66-162">响应</span><span class="sxs-lookup"><span data-stu-id="86c66-162">Response</span></span>
<span data-ttu-id="86c66-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86c66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```






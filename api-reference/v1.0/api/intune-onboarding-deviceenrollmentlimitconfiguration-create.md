---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
ms.openlocfilehash: f8fe820d63a2e6a5b3393033c49139ad85a4eb06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010111"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="1f89a-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f89a-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="1f89a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f89a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f89a-105">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f89a-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f89a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f89a-106">Prerequisites</span></span>
<span data-ttu-id="1f89a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1f89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f89a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f89a-109">Permission type</span></span>|<span data-ttu-id="1f89a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f89a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f89a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f89a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f89a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f89a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f89a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f89a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f89a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f89a-114">Not supported.</span></span>|
|<span data-ttu-id="1f89a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f89a-115">Application</span></span>|<span data-ttu-id="1f89a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f89a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f89a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f89a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f89a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f89a-118">Request headers</span></span>
|<span data-ttu-id="1f89a-119">标头</span><span class="sxs-lookup"><span data-stu-id="1f89a-119">Header</span></span>|<span data-ttu-id="1f89a-120">值</span><span class="sxs-lookup"><span data-stu-id="1f89a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f89a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f89a-121">Authorization</span></span>|<span data-ttu-id="1f89a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f89a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f89a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1f89a-123">Accept</span></span>|<span data-ttu-id="1f89a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f89a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f89a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f89a-125">Request body</span></span>
<span data-ttu-id="1f89a-126">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f89a-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="1f89a-127">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f89a-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="1f89a-128">属性</span><span class="sxs-lookup"><span data-stu-id="1f89a-128">Property</span></span>|<span data-ttu-id="1f89a-129">类型</span><span class="sxs-lookup"><span data-stu-id="1f89a-129">Type</span></span>|<span data-ttu-id="1f89a-130">说明</span><span class="sxs-lookup"><span data-stu-id="1f89a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f89a-131">id</span><span class="sxs-lookup"><span data-stu-id="1f89a-131">id</span></span>|<span data-ttu-id="1f89a-132">String</span><span class="sxs-lookup"><span data-stu-id="1f89a-132">String</span></span>|<span data-ttu-id="1f89a-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1f89a-134">displayName</span></span>|<span data-ttu-id="1f89a-135">String</span><span class="sxs-lookup"><span data-stu-id="1f89a-135">String</span></span>|<span data-ttu-id="1f89a-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-137">description</span><span class="sxs-lookup"><span data-stu-id="1f89a-137">description</span></span>|<span data-ttu-id="1f89a-138">String</span><span class="sxs-lookup"><span data-stu-id="1f89a-138">String</span></span>|<span data-ttu-id="1f89a-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-140">priority</span><span class="sxs-lookup"><span data-stu-id="1f89a-140">priority</span></span>|<span data-ttu-id="1f89a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1f89a-141">Int32</span></span>|<span data-ttu-id="1f89a-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f89a-143">createdDateTime</span></span>|<span data-ttu-id="1f89a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f89a-144">DateTimeOffset</span></span>|<span data-ttu-id="1f89a-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f89a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1f89a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f89a-147">DateTimeOffset</span></span>|<span data-ttu-id="1f89a-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-149">version</span><span class="sxs-lookup"><span data-stu-id="1f89a-149">version</span></span>|<span data-ttu-id="1f89a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1f89a-150">Int32</span></span>|<span data-ttu-id="1f89a-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f89a-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f89a-152">limit</span><span class="sxs-lookup"><span data-stu-id="1f89a-152">limit</span></span>|<span data-ttu-id="1f89a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1f89a-153">Int32</span></span>|<span data-ttu-id="1f89a-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1f89a-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1f89a-155">响应</span><span class="sxs-lookup"><span data-stu-id="1f89a-155">Response</span></span>
<span data-ttu-id="1f89a-156">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f89a-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f89a-157">示例</span><span class="sxs-lookup"><span data-stu-id="1f89a-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f89a-158">请求</span><span class="sxs-lookup"><span data-stu-id="1f89a-158">Request</span></span>
<span data-ttu-id="1f89a-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f89a-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="1f89a-160">响应</span><span class="sxs-lookup"><span data-stu-id="1f89a-160">Response</span></span>
<span data-ttu-id="1f89a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f89a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




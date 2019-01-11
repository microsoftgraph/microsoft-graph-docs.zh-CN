---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd4b1c581260a7cd1438ddad6bc2e486af1ac679
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832885"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="581af-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="581af-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="581af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="581af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="581af-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="581af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="581af-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="581af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="581af-107">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="581af-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="581af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="581af-108">Prerequisites</span></span>
<span data-ttu-id="581af-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="581af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="581af-111">Permission type</span></span>|<span data-ttu-id="581af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="581af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="581af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="581af-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="581af-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="581af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="581af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="581af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="581af-116">Not supported.</span></span>|
|<span data-ttu-id="581af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="581af-117">Application</span></span>|<span data-ttu-id="581af-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="581af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="581af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="581af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="581af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="581af-120">Request headers</span></span>
|<span data-ttu-id="581af-121">标头</span><span class="sxs-lookup"><span data-stu-id="581af-121">Header</span></span>|<span data-ttu-id="581af-122">值</span><span class="sxs-lookup"><span data-stu-id="581af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="581af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="581af-123">Authorization</span></span>|<span data-ttu-id="581af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="581af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="581af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="581af-125">Accept</span></span>|<span data-ttu-id="581af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="581af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="581af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="581af-127">Request body</span></span>
<span data-ttu-id="581af-128">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="581af-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="581af-129">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="581af-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="581af-130">属性</span><span class="sxs-lookup"><span data-stu-id="581af-130">Property</span></span>|<span data-ttu-id="581af-131">类型</span><span class="sxs-lookup"><span data-stu-id="581af-131">Type</span></span>|<span data-ttu-id="581af-132">说明</span><span class="sxs-lookup"><span data-stu-id="581af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581af-133">id</span><span class="sxs-lookup"><span data-stu-id="581af-133">id</span></span>|<span data-ttu-id="581af-134">String</span><span class="sxs-lookup"><span data-stu-id="581af-134">String</span></span>|<span data-ttu-id="581af-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-136">displayName</span><span class="sxs-lookup"><span data-stu-id="581af-136">displayName</span></span>|<span data-ttu-id="581af-137">String</span><span class="sxs-lookup"><span data-stu-id="581af-137">String</span></span>|<span data-ttu-id="581af-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-139">description</span><span class="sxs-lookup"><span data-stu-id="581af-139">description</span></span>|<span data-ttu-id="581af-140">String</span><span class="sxs-lookup"><span data-stu-id="581af-140">String</span></span>|<span data-ttu-id="581af-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-142">priority</span><span class="sxs-lookup"><span data-stu-id="581af-142">priority</span></span>|<span data-ttu-id="581af-143">Int32</span><span class="sxs-lookup"><span data-stu-id="581af-143">Int32</span></span>|<span data-ttu-id="581af-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="581af-145">createdDateTime</span></span>|<span data-ttu-id="581af-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="581af-146">DateTimeOffset</span></span>|<span data-ttu-id="581af-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="581af-148">lastModifiedDateTime</span></span>|<span data-ttu-id="581af-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="581af-149">DateTimeOffset</span></span>|<span data-ttu-id="581af-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-151">version</span><span class="sxs-lookup"><span data-stu-id="581af-151">version</span></span>|<span data-ttu-id="581af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="581af-152">Int32</span></span>|<span data-ttu-id="581af-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="581af-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="581af-154">limit</span><span class="sxs-lookup"><span data-stu-id="581af-154">limit</span></span>|<span data-ttu-id="581af-155">Int32</span><span class="sxs-lookup"><span data-stu-id="581af-155">Int32</span></span>|<span data-ttu-id="581af-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="581af-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="581af-157">响应</span><span class="sxs-lookup"><span data-stu-id="581af-157">Response</span></span>
<span data-ttu-id="581af-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="581af-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="581af-159">示例</span><span class="sxs-lookup"><span data-stu-id="581af-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="581af-160">请求</span><span class="sxs-lookup"><span data-stu-id="581af-160">Request</span></span>
<span data-ttu-id="581af-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="581af-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="581af-162">响应</span><span class="sxs-lookup"><span data-stu-id="581af-162">Response</span></span>
<span data-ttu-id="581af-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="581af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






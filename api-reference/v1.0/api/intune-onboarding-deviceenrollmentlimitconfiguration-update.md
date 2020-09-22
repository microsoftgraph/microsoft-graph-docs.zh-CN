---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8173001c86ff5156fa6c382101e10ed54bb9f7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075236"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="95941-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="95941-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="95941-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95941-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95941-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95941-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95941-106">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95941-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95941-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95941-107">Prerequisites</span></span>
<span data-ttu-id="95941-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95941-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95941-110">Permission type</span></span>|<span data-ttu-id="95941-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95941-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95941-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95941-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95941-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95941-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95941-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95941-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95941-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95941-115">Not supported.</span></span>|
|<span data-ttu-id="95941-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95941-116">Application</span></span>|<span data-ttu-id="95941-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95941-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95941-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95941-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95941-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95941-119">Request headers</span></span>
|<span data-ttu-id="95941-120">标头</span><span class="sxs-lookup"><span data-stu-id="95941-120">Header</span></span>|<span data-ttu-id="95941-121">值</span><span class="sxs-lookup"><span data-stu-id="95941-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95941-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95941-122">Authorization</span></span>|<span data-ttu-id="95941-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95941-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95941-124">接受</span><span class="sxs-lookup"><span data-stu-id="95941-124">Accept</span></span>|<span data-ttu-id="95941-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95941-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95941-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95941-126">Request body</span></span>
<span data-ttu-id="95941-127">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95941-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="95941-128">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95941-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="95941-129">属性</span><span class="sxs-lookup"><span data-stu-id="95941-129">Property</span></span>|<span data-ttu-id="95941-130">类型</span><span class="sxs-lookup"><span data-stu-id="95941-130">Type</span></span>|<span data-ttu-id="95941-131">说明</span><span class="sxs-lookup"><span data-stu-id="95941-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95941-132">id</span><span class="sxs-lookup"><span data-stu-id="95941-132">id</span></span>|<span data-ttu-id="95941-133">String</span><span class="sxs-lookup"><span data-stu-id="95941-133">String</span></span>|<span data-ttu-id="95941-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-135">displayName</span><span class="sxs-lookup"><span data-stu-id="95941-135">displayName</span></span>|<span data-ttu-id="95941-136">String</span><span class="sxs-lookup"><span data-stu-id="95941-136">String</span></span>|<span data-ttu-id="95941-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-138">description</span><span class="sxs-lookup"><span data-stu-id="95941-138">description</span></span>|<span data-ttu-id="95941-139">String</span><span class="sxs-lookup"><span data-stu-id="95941-139">String</span></span>|<span data-ttu-id="95941-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-141">priority</span><span class="sxs-lookup"><span data-stu-id="95941-141">priority</span></span>|<span data-ttu-id="95941-142">Int32</span><span class="sxs-lookup"><span data-stu-id="95941-142">Int32</span></span>|<span data-ttu-id="95941-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95941-144">createdDateTime</span></span>|<span data-ttu-id="95941-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95941-145">DateTimeOffset</span></span>|<span data-ttu-id="95941-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95941-147">lastModifiedDateTime</span></span>|<span data-ttu-id="95941-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95941-148">DateTimeOffset</span></span>|<span data-ttu-id="95941-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-150">version</span><span class="sxs-lookup"><span data-stu-id="95941-150">version</span></span>|<span data-ttu-id="95941-151">Int32</span><span class="sxs-lookup"><span data-stu-id="95941-151">Int32</span></span>|<span data-ttu-id="95941-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95941-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="95941-153">limit</span><span class="sxs-lookup"><span data-stu-id="95941-153">limit</span></span>|<span data-ttu-id="95941-154">Int32</span><span class="sxs-lookup"><span data-stu-id="95941-154">Int32</span></span>|<span data-ttu-id="95941-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95941-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="95941-156">响应</span><span class="sxs-lookup"><span data-stu-id="95941-156">Response</span></span>
<span data-ttu-id="95941-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95941-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95941-158">示例</span><span class="sxs-lookup"><span data-stu-id="95941-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="95941-159">请求</span><span class="sxs-lookup"><span data-stu-id="95941-159">Request</span></span>
<span data-ttu-id="95941-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95941-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="95941-161">响应</span><span class="sxs-lookup"><span data-stu-id="95941-161">Response</span></span>
<span data-ttu-id="95941-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95941-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










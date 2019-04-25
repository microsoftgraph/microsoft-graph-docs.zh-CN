---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c54a7bba58e64fc9f74053cc40e43517bc65a881
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582785"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="29741-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="29741-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="29741-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29741-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29741-105">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="29741-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29741-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="29741-106">Prerequisites</span></span>
<span data-ttu-id="29741-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29741-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29741-109">Permission type</span></span>|<span data-ttu-id="29741-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29741-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29741-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29741-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29741-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29741-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29741-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29741-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29741-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29741-114">Not supported.</span></span>|
|<span data-ttu-id="29741-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="29741-115">Application</span></span>|<span data-ttu-id="29741-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29741-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29741-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29741-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29741-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="29741-118">Request headers</span></span>
|<span data-ttu-id="29741-119">标头</span><span class="sxs-lookup"><span data-stu-id="29741-119">Header</span></span>|<span data-ttu-id="29741-120">值</span><span class="sxs-lookup"><span data-stu-id="29741-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29741-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29741-121">Authorization</span></span>|<span data-ttu-id="29741-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29741-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29741-123">接受</span><span class="sxs-lookup"><span data-stu-id="29741-123">Accept</span></span>|<span data-ttu-id="29741-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29741-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29741-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="29741-125">Request body</span></span>
<span data-ttu-id="29741-126">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29741-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="29741-127">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29741-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="29741-128">属性</span><span class="sxs-lookup"><span data-stu-id="29741-128">Property</span></span>|<span data-ttu-id="29741-129">类型</span><span class="sxs-lookup"><span data-stu-id="29741-129">Type</span></span>|<span data-ttu-id="29741-130">说明</span><span class="sxs-lookup"><span data-stu-id="29741-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29741-131">id</span><span class="sxs-lookup"><span data-stu-id="29741-131">id</span></span>|<span data-ttu-id="29741-132">字符串</span><span class="sxs-lookup"><span data-stu-id="29741-132">String</span></span>|<span data-ttu-id="29741-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-134">displayName</span><span class="sxs-lookup"><span data-stu-id="29741-134">displayName</span></span>|<span data-ttu-id="29741-135">String</span><span class="sxs-lookup"><span data-stu-id="29741-135">String</span></span>|<span data-ttu-id="29741-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-137">说明</span><span class="sxs-lookup"><span data-stu-id="29741-137">description</span></span>|<span data-ttu-id="29741-138">String</span><span class="sxs-lookup"><span data-stu-id="29741-138">String</span></span>|<span data-ttu-id="29741-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-140">priority</span><span class="sxs-lookup"><span data-stu-id="29741-140">priority</span></span>|<span data-ttu-id="29741-141">Int32</span><span class="sxs-lookup"><span data-stu-id="29741-141">Int32</span></span>|<span data-ttu-id="29741-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29741-143">createdDateTime</span></span>|<span data-ttu-id="29741-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29741-144">DateTimeOffset</span></span>|<span data-ttu-id="29741-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29741-146">lastModifiedDateTime</span></span>|<span data-ttu-id="29741-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29741-147">DateTimeOffset</span></span>|<span data-ttu-id="29741-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-149">version</span><span class="sxs-lookup"><span data-stu-id="29741-149">version</span></span>|<span data-ttu-id="29741-150">Int32</span><span class="sxs-lookup"><span data-stu-id="29741-150">Int32</span></span>|<span data-ttu-id="29741-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29741-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29741-152">limit</span><span class="sxs-lookup"><span data-stu-id="29741-152">limit</span></span>|<span data-ttu-id="29741-153">Int32</span><span class="sxs-lookup"><span data-stu-id="29741-153">Int32</span></span>|<span data-ttu-id="29741-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29741-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29741-155">响应</span><span class="sxs-lookup"><span data-stu-id="29741-155">Response</span></span>
<span data-ttu-id="29741-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29741-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29741-157">示例</span><span class="sxs-lookup"><span data-stu-id="29741-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="29741-158">请求</span><span class="sxs-lookup"><span data-stu-id="29741-158">Request</span></span>
<span data-ttu-id="29741-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29741-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29741-160">响应</span><span class="sxs-lookup"><span data-stu-id="29741-160">Response</span></span>
<span data-ttu-id="29741-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29741-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




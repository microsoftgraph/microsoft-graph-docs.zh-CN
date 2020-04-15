---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 277cea3de8ada82e5661070eacacf345f0cc79ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451826"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="7dddc-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dddc-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="7dddc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dddc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dddc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7dddc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dddc-106">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dddc-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dddc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dddc-107">Prerequisites</span></span>
<span data-ttu-id="7dddc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dddc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dddc-110">Permission type</span></span>|<span data-ttu-id="7dddc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dddc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dddc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dddc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dddc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dddc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7dddc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dddc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dddc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dddc-115">Not supported.</span></span>|
|<span data-ttu-id="7dddc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dddc-116">Application</span></span>|<span data-ttu-id="7dddc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dddc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dddc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dddc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7dddc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dddc-119">Request headers</span></span>
|<span data-ttu-id="7dddc-120">标头</span><span class="sxs-lookup"><span data-stu-id="7dddc-120">Header</span></span>|<span data-ttu-id="7dddc-121">值</span><span class="sxs-lookup"><span data-stu-id="7dddc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dddc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dddc-122">Authorization</span></span>|<span data-ttu-id="7dddc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dddc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dddc-124">接受</span><span class="sxs-lookup"><span data-stu-id="7dddc-124">Accept</span></span>|<span data-ttu-id="7dddc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7dddc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dddc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dddc-126">Request body</span></span>
<span data-ttu-id="7dddc-127">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dddc-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="7dddc-128">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dddc-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="7dddc-129">属性</span><span class="sxs-lookup"><span data-stu-id="7dddc-129">Property</span></span>|<span data-ttu-id="7dddc-130">类型</span><span class="sxs-lookup"><span data-stu-id="7dddc-130">Type</span></span>|<span data-ttu-id="7dddc-131">说明</span><span class="sxs-lookup"><span data-stu-id="7dddc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dddc-132">id</span><span class="sxs-lookup"><span data-stu-id="7dddc-132">id</span></span>|<span data-ttu-id="7dddc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7dddc-133">String</span></span>|<span data-ttu-id="7dddc-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7dddc-135">displayName</span></span>|<span data-ttu-id="7dddc-136">String</span><span class="sxs-lookup"><span data-stu-id="7dddc-136">String</span></span>|<span data-ttu-id="7dddc-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-138">description</span><span class="sxs-lookup"><span data-stu-id="7dddc-138">description</span></span>|<span data-ttu-id="7dddc-139">String</span><span class="sxs-lookup"><span data-stu-id="7dddc-139">String</span></span>|<span data-ttu-id="7dddc-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-141">priority</span><span class="sxs-lookup"><span data-stu-id="7dddc-141">priority</span></span>|<span data-ttu-id="7dddc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7dddc-142">Int32</span></span>|<span data-ttu-id="7dddc-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dddc-144">createdDateTime</span></span>|<span data-ttu-id="7dddc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dddc-145">DateTimeOffset</span></span>|<span data-ttu-id="7dddc-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dddc-147">lastModifiedDateTime</span></span>|<span data-ttu-id="7dddc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dddc-148">DateTimeOffset</span></span>|<span data-ttu-id="7dddc-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-150">version</span><span class="sxs-lookup"><span data-stu-id="7dddc-150">version</span></span>|<span data-ttu-id="7dddc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7dddc-151">Int32</span></span>|<span data-ttu-id="7dddc-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dddc-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7dddc-153">limit</span><span class="sxs-lookup"><span data-stu-id="7dddc-153">limit</span></span>|<span data-ttu-id="7dddc-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7dddc-154">Int32</span></span>|<span data-ttu-id="7dddc-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7dddc-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7dddc-156">响应</span><span class="sxs-lookup"><span data-stu-id="7dddc-156">Response</span></span>
<span data-ttu-id="7dddc-157">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dddc-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dddc-158">示例</span><span class="sxs-lookup"><span data-stu-id="7dddc-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dddc-159">请求</span><span class="sxs-lookup"><span data-stu-id="7dddc-159">Request</span></span>
<span data-ttu-id="7dddc-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dddc-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7dddc-161">响应</span><span class="sxs-lookup"><span data-stu-id="7dddc-161">Response</span></span>
<span data-ttu-id="7dddc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dddc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







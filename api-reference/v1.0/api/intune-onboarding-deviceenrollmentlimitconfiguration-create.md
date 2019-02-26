---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d6773086a44205a3ddb2c5603e2a898c5bfab10
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262151"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="f4a85-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4a85-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="f4a85-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4a85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a85-105">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4a85-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4a85-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4a85-106">Prerequisites</span></span>
<span data-ttu-id="f4a85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f4a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4a85-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4a85-109">Permission type</span></span>|<span data-ttu-id="f4a85-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4a85-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a85-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4a85-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a85-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4a85-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a85-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a85-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4a85-114">Not supported.</span></span>|
|<span data-ttu-id="f4a85-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4a85-115">Application</span></span>|<span data-ttu-id="f4a85-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4a85-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a85-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4a85-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f4a85-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4a85-118">Request headers</span></span>
|<span data-ttu-id="f4a85-119">标头</span><span class="sxs-lookup"><span data-stu-id="f4a85-119">Header</span></span>|<span data-ttu-id="f4a85-120">值</span><span class="sxs-lookup"><span data-stu-id="f4a85-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a85-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a85-121">Authorization</span></span>|<span data-ttu-id="f4a85-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4a85-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a85-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f4a85-123">Accept</span></span>|<span data-ttu-id="f4a85-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a85-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a85-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4a85-125">Request body</span></span>
<span data-ttu-id="f4a85-126">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4a85-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="f4a85-127">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4a85-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="f4a85-128">属性</span><span class="sxs-lookup"><span data-stu-id="f4a85-128">Property</span></span>|<span data-ttu-id="f4a85-129">类型</span><span class="sxs-lookup"><span data-stu-id="f4a85-129">Type</span></span>|<span data-ttu-id="f4a85-130">说明</span><span class="sxs-lookup"><span data-stu-id="f4a85-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a85-131">id</span><span class="sxs-lookup"><span data-stu-id="f4a85-131">id</span></span>|<span data-ttu-id="f4a85-132">String</span><span class="sxs-lookup"><span data-stu-id="f4a85-132">String</span></span>|<span data-ttu-id="f4a85-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f4a85-134">displayName</span></span>|<span data-ttu-id="f4a85-135">String</span><span class="sxs-lookup"><span data-stu-id="f4a85-135">String</span></span>|<span data-ttu-id="f4a85-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-137">description</span><span class="sxs-lookup"><span data-stu-id="f4a85-137">description</span></span>|<span data-ttu-id="f4a85-138">String</span><span class="sxs-lookup"><span data-stu-id="f4a85-138">String</span></span>|<span data-ttu-id="f4a85-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-140">priority</span><span class="sxs-lookup"><span data-stu-id="f4a85-140">priority</span></span>|<span data-ttu-id="f4a85-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f4a85-141">Int32</span></span>|<span data-ttu-id="f4a85-142">尚未记录 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4a85-143">createdDateTime</span></span>|<span data-ttu-id="f4a85-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4a85-144">DateTimeOffset</span></span>|<span data-ttu-id="f4a85-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4a85-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f4a85-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4a85-147">DateTimeOffset</span></span>|<span data-ttu-id="f4a85-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-149">version</span><span class="sxs-lookup"><span data-stu-id="f4a85-149">version</span></span>|<span data-ttu-id="f4a85-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f4a85-150">Int32</span></span>|<span data-ttu-id="f4a85-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4a85-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f4a85-152">limit</span><span class="sxs-lookup"><span data-stu-id="f4a85-152">limit</span></span>|<span data-ttu-id="f4a85-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f4a85-153">Int32</span></span>|<span data-ttu-id="f4a85-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4a85-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f4a85-155">响应</span><span class="sxs-lookup"><span data-stu-id="f4a85-155">Response</span></span>
<span data-ttu-id="f4a85-156">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4a85-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4a85-157">示例</span><span class="sxs-lookup"><span data-stu-id="f4a85-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a85-158">请求</span><span class="sxs-lookup"><span data-stu-id="f4a85-158">Request</span></span>
<span data-ttu-id="f4a85-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4a85-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4a85-160">响应</span><span class="sxs-lookup"><span data-stu-id="f4a85-160">Response</span></span>
<span data-ttu-id="f4a85-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4a85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a331e49ea65450012d5f632b88579044382c9a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986374"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="3f67f-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="3f67f-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="3f67f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f67f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f67f-105">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f67f-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f67f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f67f-106">Prerequisites</span></span>
<span data-ttu-id="3f67f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f67f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f67f-109">Permission type</span></span>|<span data-ttu-id="3f67f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f67f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f67f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f67f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f67f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f67f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f67f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f67f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f67f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f67f-114">Not supported.</span></span>|
|<span data-ttu-id="3f67f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f67f-115">Application</span></span>|<span data-ttu-id="3f67f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f67f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f67f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f67f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f67f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f67f-118">Request headers</span></span>
|<span data-ttu-id="3f67f-119">标头</span><span class="sxs-lookup"><span data-stu-id="3f67f-119">Header</span></span>|<span data-ttu-id="3f67f-120">值</span><span class="sxs-lookup"><span data-stu-id="3f67f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f67f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f67f-121">Authorization</span></span>|<span data-ttu-id="3f67f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f67f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f67f-123">接受</span><span class="sxs-lookup"><span data-stu-id="3f67f-123">Accept</span></span>|<span data-ttu-id="3f67f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3f67f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f67f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f67f-125">Request body</span></span>
<span data-ttu-id="3f67f-126">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f67f-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="3f67f-127">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3f67f-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="3f67f-128">属性</span><span class="sxs-lookup"><span data-stu-id="3f67f-128">Property</span></span>|<span data-ttu-id="3f67f-129">类型</span><span class="sxs-lookup"><span data-stu-id="3f67f-129">Type</span></span>|<span data-ttu-id="3f67f-130">说明</span><span class="sxs-lookup"><span data-stu-id="3f67f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f67f-131">id</span><span class="sxs-lookup"><span data-stu-id="3f67f-131">id</span></span>|<span data-ttu-id="3f67f-132">String</span><span class="sxs-lookup"><span data-stu-id="3f67f-132">String</span></span>|<span data-ttu-id="3f67f-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3f67f-134">displayName</span></span>|<span data-ttu-id="3f67f-135">String</span><span class="sxs-lookup"><span data-stu-id="3f67f-135">String</span></span>|<span data-ttu-id="3f67f-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-137">description</span><span class="sxs-lookup"><span data-stu-id="3f67f-137">description</span></span>|<span data-ttu-id="3f67f-138">String</span><span class="sxs-lookup"><span data-stu-id="3f67f-138">String</span></span>|<span data-ttu-id="3f67f-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-140">priority</span><span class="sxs-lookup"><span data-stu-id="3f67f-140">priority</span></span>|<span data-ttu-id="3f67f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3f67f-141">Int32</span></span>|<span data-ttu-id="3f67f-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f67f-143">createdDateTime</span></span>|<span data-ttu-id="3f67f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f67f-144">DateTimeOffset</span></span>|<span data-ttu-id="3f67f-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f67f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="3f67f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f67f-147">DateTimeOffset</span></span>|<span data-ttu-id="3f67f-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-149">version</span><span class="sxs-lookup"><span data-stu-id="3f67f-149">version</span></span>|<span data-ttu-id="3f67f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3f67f-150">Int32</span></span>|<span data-ttu-id="3f67f-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f67f-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3f67f-152">limit</span><span class="sxs-lookup"><span data-stu-id="3f67f-152">limit</span></span>|<span data-ttu-id="3f67f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3f67f-153">Int32</span></span>|<span data-ttu-id="3f67f-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f67f-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f67f-155">响应</span><span class="sxs-lookup"><span data-stu-id="3f67f-155">Response</span></span>
<span data-ttu-id="3f67f-156">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f67f-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f67f-157">示例</span><span class="sxs-lookup"><span data-stu-id="3f67f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f67f-158">请求</span><span class="sxs-lookup"><span data-stu-id="3f67f-158">Request</span></span>
<span data-ttu-id="3f67f-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f67f-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f67f-160">响应</span><span class="sxs-lookup"><span data-stu-id="3f67f-160">Response</span></span>
<span data-ttu-id="3f67f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f67f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: 更新 userExperienceAnalyticsBaseline
description: 更新 userExperienceAnalyticsBaseline 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbf41a82332d638880913246c974ac36298cc7de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011163"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="d931f-103">更新 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="d931f-103">Update userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="d931f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d931f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d931f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d931f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d931f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d931f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d931f-107">更新 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d931f-107">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d931f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d931f-108">Prerequisites</span></span>
<span data-ttu-id="d931f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d931f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d931f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d931f-111">Permission type</span></span>|<span data-ttu-id="d931f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d931f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d931f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d931f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d931f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d931f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d931f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d931f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d931f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d931f-116">Not supported.</span></span>|
|<span data-ttu-id="d931f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d931f-117">Application</span></span>|<span data-ttu-id="d931f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d931f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d931f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d931f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="d931f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d931f-120">Request headers</span></span>
|<span data-ttu-id="d931f-121">标头</span><span class="sxs-lookup"><span data-stu-id="d931f-121">Header</span></span>|<span data-ttu-id="d931f-122">值</span><span class="sxs-lookup"><span data-stu-id="d931f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d931f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d931f-123">Authorization</span></span>|<span data-ttu-id="d931f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d931f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d931f-125">接受</span><span class="sxs-lookup"><span data-stu-id="d931f-125">Accept</span></span>|<span data-ttu-id="d931f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d931f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d931f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d931f-127">Request body</span></span>
<span data-ttu-id="d931f-128">在请求正文中，提供 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d931f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="d931f-129">下表显示创建 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d931f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="d931f-130">属性</span><span class="sxs-lookup"><span data-stu-id="d931f-130">Property</span></span>|<span data-ttu-id="d931f-131">类型</span><span class="sxs-lookup"><span data-stu-id="d931f-131">Type</span></span>|<span data-ttu-id="d931f-132">说明</span><span class="sxs-lookup"><span data-stu-id="d931f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d931f-133">id</span><span class="sxs-lookup"><span data-stu-id="d931f-133">id</span></span>|<span data-ttu-id="d931f-134">String</span><span class="sxs-lookup"><span data-stu-id="d931f-134">String</span></span>|<span data-ttu-id="d931f-135">User experience analytics 比较基准的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d931f-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="d931f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d931f-136">displayName</span></span>|<span data-ttu-id="d931f-137">String</span><span class="sxs-lookup"><span data-stu-id="d931f-137">String</span></span>|<span data-ttu-id="d931f-138">User experience analytics 基线的名称。</span><span class="sxs-lookup"><span data-stu-id="d931f-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="d931f-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="d931f-139">overallScore</span></span>|<span data-ttu-id="d931f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d931f-140">Int32</span></span>|<span data-ttu-id="d931f-141">用户体验分析基准的总体分数。</span><span class="sxs-lookup"><span data-stu-id="d931f-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="d931f-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d931f-142">isBuiltIn</span></span>|<span data-ttu-id="d931f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d931f-143">Boolean</span></span>|<span data-ttu-id="d931f-144">指示当前基线是商业中间基线还是自定义基线。</span><span class="sxs-lookup"><span data-stu-id="d931f-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="d931f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d931f-145">createdDateTime</span></span>|<span data-ttu-id="d931f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d931f-146">DateTimeOffset</span></span>|<span data-ttu-id="d931f-147">自定义基线的创建日期。</span><span class="sxs-lookup"><span data-stu-id="d931f-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="d931f-148">响应</span><span class="sxs-lookup"><span data-stu-id="d931f-148">Response</span></span>
<span data-ttu-id="d931f-149">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d931f-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d931f-150">示例</span><span class="sxs-lookup"><span data-stu-id="d931f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d931f-151">请求</span><span class="sxs-lookup"><span data-stu-id="d931f-151">Request</span></span>
<span data-ttu-id="d931f-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d931f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="d931f-153">响应</span><span class="sxs-lookup"><span data-stu-id="d931f-153">Response</span></span>
<span data-ttu-id="d931f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d931f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
}
```







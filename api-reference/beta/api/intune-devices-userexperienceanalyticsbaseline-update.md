---
title: 更新 userExperienceAnalyticsBaseline
description: 更新 userExperienceAnalyticsBaseline 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f8a91c0b0a70437d2a2ccee39d8afdd35d73aee
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944531"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="a6b76-103">更新 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="a6b76-103">Update userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="a6b76-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6b76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6b76-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6b76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6b76-106">更新[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6b76-106">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6b76-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6b76-107">Prerequisites</span></span>
<span data-ttu-id="a6b76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6b76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b76-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6b76-110">Permission type</span></span>|<span data-ttu-id="a6b76-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6b76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6b76-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6b76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6b76-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b76-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a6b76-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6b76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6b76-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6b76-115">Not supported.</span></span>|
|<span data-ttu-id="a6b76-116">Application</span><span class="sxs-lookup"><span data-stu-id="a6b76-116">Application</span></span>|<span data-ttu-id="a6b76-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b76-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b76-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6b76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="a6b76-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6b76-119">Request headers</span></span>
|<span data-ttu-id="a6b76-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6b76-120">Header</span></span>|<span data-ttu-id="a6b76-121">值</span><span class="sxs-lookup"><span data-stu-id="a6b76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6b76-122">授权</span><span class="sxs-lookup"><span data-stu-id="a6b76-122">Authorization</span></span>|<span data-ttu-id="a6b76-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6b76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6b76-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6b76-124">Accept</span></span>|<span data-ttu-id="a6b76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6b76-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6b76-126">Request body</span></span>
<span data-ttu-id="a6b76-127">在请求正文中，提供[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b76-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="a6b76-128">下表显示创建[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6b76-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="a6b76-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6b76-129">Property</span></span>|<span data-ttu-id="a6b76-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6b76-130">Type</span></span>|<span data-ttu-id="a6b76-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6b76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b76-132">id</span><span class="sxs-lookup"><span data-stu-id="a6b76-132">id</span></span>|<span data-ttu-id="a6b76-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a6b76-133">String</span></span>|<span data-ttu-id="a6b76-134">User experience analytics 比较基准的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b76-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a6b76-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a6b76-135">displayName</span></span>|<span data-ttu-id="a6b76-136">String</span><span class="sxs-lookup"><span data-stu-id="a6b76-136">String</span></span>|<span data-ttu-id="a6b76-137">User experience analytics 基线的名称。</span><span class="sxs-lookup"><span data-stu-id="a6b76-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a6b76-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="a6b76-138">overallScore</span></span>|<span data-ttu-id="a6b76-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a6b76-139">Int32</span></span>|<span data-ttu-id="a6b76-140">用户体验分析基准的总体分数。</span><span class="sxs-lookup"><span data-stu-id="a6b76-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a6b76-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a6b76-141">isBuiltIn</span></span>|<span data-ttu-id="a6b76-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6b76-142">Boolean</span></span>|<span data-ttu-id="a6b76-143">指示当前基线是商业中间基线还是自定义基线。</span><span class="sxs-lookup"><span data-stu-id="a6b76-143">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="a6b76-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6b76-144">createdDateTime</span></span>|<span data-ttu-id="a6b76-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6b76-145">DateTimeOffset</span></span>|<span data-ttu-id="a6b76-146">自定义基线的创建日期。</span><span class="sxs-lookup"><span data-stu-id="a6b76-146">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="a6b76-147">响应</span><span class="sxs-lookup"><span data-stu-id="a6b76-147">Response</span></span>
<span data-ttu-id="a6b76-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6b76-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b76-149">示例</span><span class="sxs-lookup"><span data-stu-id="a6b76-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6b76-150">请求</span><span class="sxs-lookup"><span data-stu-id="a6b76-150">Request</span></span>
<span data-ttu-id="a6b76-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6b76-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6b76-152">响应</span><span class="sxs-lookup"><span data-stu-id="a6b76-152">Response</span></span>
<span data-ttu-id="a6b76-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6b76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






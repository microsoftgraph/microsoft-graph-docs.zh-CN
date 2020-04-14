---
title: 创建 userExperienceAnalyticsBaseline
description: 创建新的 userExperienceAnalyticsBaseline 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c11f14f2a281ab2317645a71abc0effaf541fb0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43323442"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="9ebe6-103">创建 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="9ebe6-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="9ebe6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ebe6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ebe6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ebe6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ebe6-107">创建新的[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ebe6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ebe6-108">Prerequisites</span></span>
<span data-ttu-id="9ebe6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ebe6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ebe6-111">Permission type</span></span>|<span data-ttu-id="9ebe6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ebe6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ebe6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ebe6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ebe6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ebe6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9ebe6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ebe6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ebe6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-116">Not supported.</span></span>|
|<span data-ttu-id="9ebe6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ebe6-117">Application</span></span>|<span data-ttu-id="9ebe6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ebe6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ebe6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ebe6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="9ebe6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ebe6-120">Request headers</span></span>
|<span data-ttu-id="9ebe6-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ebe6-121">Header</span></span>|<span data-ttu-id="9ebe6-122">值</span><span class="sxs-lookup"><span data-stu-id="9ebe6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ebe6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ebe6-123">Authorization</span></span>|<span data-ttu-id="9ebe6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ebe6-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ebe6-125">Accept</span></span>|<span data-ttu-id="9ebe6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ebe6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ebe6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ebe6-127">Request body</span></span>
<span data-ttu-id="9ebe6-128">在请求正文中，提供 userExperienceAnalyticsBaseline 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="9ebe6-129">下表显示创建 userExperienceAnalyticsBaseline 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="9ebe6-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ebe6-130">Property</span></span>|<span data-ttu-id="9ebe6-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ebe6-131">Type</span></span>|<span data-ttu-id="9ebe6-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ebe6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ebe6-133">id</span><span class="sxs-lookup"><span data-stu-id="9ebe6-133">id</span></span>|<span data-ttu-id="9ebe6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9ebe6-134">String</span></span>|<span data-ttu-id="9ebe6-135">User experience analytics 比较基准的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="9ebe6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9ebe6-136">displayName</span></span>|<span data-ttu-id="9ebe6-137">String</span><span class="sxs-lookup"><span data-stu-id="9ebe6-137">String</span></span>|<span data-ttu-id="9ebe6-138">User experience analytics 基线的名称。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="9ebe6-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="9ebe6-139">overallScore</span></span>|<span data-ttu-id="9ebe6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9ebe6-140">Int32</span></span>|<span data-ttu-id="9ebe6-141">用户体验分析基准的总体分数。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="9ebe6-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9ebe6-142">isBuiltIn</span></span>|<span data-ttu-id="9ebe6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ebe6-143">Boolean</span></span>|<span data-ttu-id="9ebe6-144">指示当前基线是商业中间基线还是自定义基线。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="9ebe6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ebe6-145">createdDateTime</span></span>|<span data-ttu-id="9ebe6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ebe6-146">DateTimeOffset</span></span>|<span data-ttu-id="9ebe6-147">自定义基线的创建日期。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="9ebe6-148">响应</span><span class="sxs-lookup"><span data-stu-id="9ebe6-148">Response</span></span>
<span data-ttu-id="9ebe6-149">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ebe6-150">示例</span><span class="sxs-lookup"><span data-stu-id="9ebe6-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ebe6-151">请求</span><span class="sxs-lookup"><span data-stu-id="9ebe6-151">Request</span></span>
<span data-ttu-id="9ebe6-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="9ebe6-153">响应</span><span class="sxs-lookup"><span data-stu-id="9ebe6-153">Response</span></span>
<span data-ttu-id="9ebe6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ebe6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




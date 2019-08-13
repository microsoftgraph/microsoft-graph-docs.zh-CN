---
title: 创建 userExperienceAnalyticsBaseline
description: 创建新的 userExperienceAnalyticsBaseline 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1877d4f6cc964e311025a10988803723b1806510
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350440"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="00c74-103">创建 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="00c74-103">Create userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="00c74-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00c74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00c74-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00c74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00c74-106">创建新的[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00c74-106">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00c74-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="00c74-107">Prerequisites</span></span>
<span data-ttu-id="00c74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00c74-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00c74-110">Permission type</span></span>|<span data-ttu-id="00c74-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00c74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00c74-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00c74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00c74-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00c74-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="00c74-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00c74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00c74-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00c74-115">Not supported.</span></span>|
|<span data-ttu-id="00c74-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00c74-116">Application</span></span>|<span data-ttu-id="00c74-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00c74-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00c74-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00c74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="00c74-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00c74-119">Request headers</span></span>
|<span data-ttu-id="00c74-120">标头</span><span class="sxs-lookup"><span data-stu-id="00c74-120">Header</span></span>|<span data-ttu-id="00c74-121">值</span><span class="sxs-lookup"><span data-stu-id="00c74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00c74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00c74-122">Authorization</span></span>|<span data-ttu-id="00c74-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00c74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00c74-124">接受</span><span class="sxs-lookup"><span data-stu-id="00c74-124">Accept</span></span>|<span data-ttu-id="00c74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00c74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00c74-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="00c74-126">Request body</span></span>
<span data-ttu-id="00c74-127">在请求正文中, 提供 userExperienceAnalyticsBaseline 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00c74-127">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="00c74-128">下表显示创建 userExperienceAnalyticsBaseline 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00c74-128">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="00c74-129">属性</span><span class="sxs-lookup"><span data-stu-id="00c74-129">Property</span></span>|<span data-ttu-id="00c74-130">类型</span><span class="sxs-lookup"><span data-stu-id="00c74-130">Type</span></span>|<span data-ttu-id="00c74-131">说明</span><span class="sxs-lookup"><span data-stu-id="00c74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00c74-132">id</span><span class="sxs-lookup"><span data-stu-id="00c74-132">id</span></span>|<span data-ttu-id="00c74-133">String</span><span class="sxs-lookup"><span data-stu-id="00c74-133">String</span></span>|<span data-ttu-id="00c74-134">User experience analytics 比较基准的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00c74-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="00c74-135">displayName</span><span class="sxs-lookup"><span data-stu-id="00c74-135">displayName</span></span>|<span data-ttu-id="00c74-136">String</span><span class="sxs-lookup"><span data-stu-id="00c74-136">String</span></span>|<span data-ttu-id="00c74-137">User experience analytics 基线的名称。</span><span class="sxs-lookup"><span data-stu-id="00c74-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="00c74-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="00c74-138">overallScore</span></span>|<span data-ttu-id="00c74-139">Int32</span><span class="sxs-lookup"><span data-stu-id="00c74-139">Int32</span></span>|<span data-ttu-id="00c74-140">用户体验分析基准的总体分数。</span><span class="sxs-lookup"><span data-stu-id="00c74-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="00c74-141">overallRegressionThreshold</span><span class="sxs-lookup"><span data-stu-id="00c74-141">overallRegressionThreshold</span></span>|<span data-ttu-id="00c74-142">Int32</span><span class="sxs-lookup"><span data-stu-id="00c74-142">Int32</span></span>|<span data-ttu-id="00c74-143">User experience analytics 比较基准的总体回归阈值。</span><span class="sxs-lookup"><span data-stu-id="00c74-143">The overall regression threshold of the user experience analytics baseline.</span></span>|



## <a name="response"></a><span data-ttu-id="00c74-144">响应</span><span class="sxs-lookup"><span data-stu-id="00c74-144">Response</span></span>
<span data-ttu-id="00c74-145">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00c74-145">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00c74-146">示例</span><span class="sxs-lookup"><span data-stu-id="00c74-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="00c74-147">请求</span><span class="sxs-lookup"><span data-stu-id="00c74-147">Request</span></span>
<span data-ttu-id="00c74-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00c74-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```

### <a name="response"></a><span data-ttu-id="00c74-149">响应</span><span class="sxs-lookup"><span data-stu-id="00c74-149">Response</span></span>
<span data-ttu-id="00c74-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00c74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```







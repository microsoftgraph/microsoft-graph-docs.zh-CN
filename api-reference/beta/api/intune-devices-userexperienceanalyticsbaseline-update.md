---
title: 更新 userExperienceAnalyticsBaseline
description: 更新 userExperienceAnalyticsBaseline 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4594b56e33ff8cf7d8583c1233d5e0083bf6bcd1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154285"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="14f26-103">更新 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="14f26-103">Update userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="14f26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14f26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14f26-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14f26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14f26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14f26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14f26-107">更新 [userExperienceAnalyticsBaseline 对象](../resources/intune-devices-userexperienceanalyticsbaseline.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="14f26-107">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14f26-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="14f26-108">Prerequisites</span></span>
<span data-ttu-id="14f26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14f26-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14f26-111">Permission type</span></span>|<span data-ttu-id="14f26-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14f26-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14f26-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14f26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14f26-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f26-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14f26-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14f26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14f26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14f26-116">Not supported.</span></span>|
|<span data-ttu-id="14f26-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="14f26-117">Application</span></span>|<span data-ttu-id="14f26-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f26-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14f26-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14f26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="14f26-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14f26-120">Request headers</span></span>
|<span data-ttu-id="14f26-121">标头</span><span class="sxs-lookup"><span data-stu-id="14f26-121">Header</span></span>|<span data-ttu-id="14f26-122">值</span><span class="sxs-lookup"><span data-stu-id="14f26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14f26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14f26-123">Authorization</span></span>|<span data-ttu-id="14f26-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14f26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14f26-125">接受</span><span class="sxs-lookup"><span data-stu-id="14f26-125">Accept</span></span>|<span data-ttu-id="14f26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14f26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14f26-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14f26-127">Request body</span></span>
<span data-ttu-id="14f26-128">在请求正文中，提供 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14f26-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="14f26-129">下表显示创建 [userExperienceAnalyticsBaseline 时所需的属性](../resources/intune-devices-userexperienceanalyticsbaseline.md)。</span><span class="sxs-lookup"><span data-stu-id="14f26-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="14f26-130">属性</span><span class="sxs-lookup"><span data-stu-id="14f26-130">Property</span></span>|<span data-ttu-id="14f26-131">类型</span><span class="sxs-lookup"><span data-stu-id="14f26-131">Type</span></span>|<span data-ttu-id="14f26-132">说明</span><span class="sxs-lookup"><span data-stu-id="14f26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14f26-133">id</span><span class="sxs-lookup"><span data-stu-id="14f26-133">id</span></span>|<span data-ttu-id="14f26-134">String</span><span class="sxs-lookup"><span data-stu-id="14f26-134">String</span></span>|<span data-ttu-id="14f26-135">用户体验分析基线的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14f26-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="14f26-136">displayName</span><span class="sxs-lookup"><span data-stu-id="14f26-136">displayName</span></span>|<span data-ttu-id="14f26-137">String</span><span class="sxs-lookup"><span data-stu-id="14f26-137">String</span></span>|<span data-ttu-id="14f26-138">用户体验分析基线的名称。</span><span class="sxs-lookup"><span data-stu-id="14f26-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="14f26-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="14f26-139">overallScore</span></span>|<span data-ttu-id="14f26-140">Int32</span><span class="sxs-lookup"><span data-stu-id="14f26-140">Int32</span></span>|<span data-ttu-id="14f26-141">用户体验分析基线的整体分数。</span><span class="sxs-lookup"><span data-stu-id="14f26-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="14f26-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="14f26-142">isBuiltIn</span></span>|<span data-ttu-id="14f26-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="14f26-143">Boolean</span></span>|<span data-ttu-id="14f26-144">表示当前比较基准是商业中值基线还是自定义比较基准。</span><span class="sxs-lookup"><span data-stu-id="14f26-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="14f26-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14f26-145">createdDateTime</span></span>|<span data-ttu-id="14f26-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f26-146">DateTimeOffset</span></span>|<span data-ttu-id="14f26-147">创建自定义比较基准的日期。</span><span class="sxs-lookup"><span data-stu-id="14f26-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="14f26-148">响应</span><span class="sxs-lookup"><span data-stu-id="14f26-148">Response</span></span>
<span data-ttu-id="14f26-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14f26-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14f26-150">示例</span><span class="sxs-lookup"><span data-stu-id="14f26-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="14f26-151">请求</span><span class="sxs-lookup"><span data-stu-id="14f26-151">Request</span></span>
<span data-ttu-id="14f26-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14f26-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14f26-153">响应</span><span class="sxs-lookup"><span data-stu-id="14f26-153">Response</span></span>
<span data-ttu-id="14f26-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14f26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





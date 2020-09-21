---
title: 创建 userExperienceAnalyticsMetricHistory
description: 创建新的 userExperienceAnalyticsMetricHistory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b5f02c4cb7558c3c3e18661e3978a16227d23b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970108"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="b9976-103">创建 userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="b9976-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="b9976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9976-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9976-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9976-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9976-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9976-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9976-107">创建新的 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9976-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9976-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9976-108">Prerequisites</span></span>
<span data-ttu-id="b9976-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9976-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9976-111">Permission type</span></span>|<span data-ttu-id="b9976-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9976-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9976-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9976-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9976-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9976-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b9976-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9976-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9976-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9976-116">Not supported.</span></span>|
|<span data-ttu-id="b9976-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9976-117">Application</span></span>|<span data-ttu-id="b9976-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9976-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9976-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9976-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="b9976-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9976-120">Request headers</span></span>
|<span data-ttu-id="b9976-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9976-121">Header</span></span>|<span data-ttu-id="b9976-122">值</span><span class="sxs-lookup"><span data-stu-id="b9976-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9976-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9976-123">Authorization</span></span>|<span data-ttu-id="b9976-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9976-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9976-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9976-125">Accept</span></span>|<span data-ttu-id="b9976-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9976-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9976-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9976-127">Request body</span></span>
<span data-ttu-id="b9976-128">在请求正文中，提供 userExperienceAnalyticsMetricHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9976-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="b9976-129">下表显示创建 userExperienceAnalyticsMetricHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9976-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="b9976-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9976-130">Property</span></span>|<span data-ttu-id="b9976-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9976-131">Type</span></span>|<span data-ttu-id="b9976-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9976-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9976-133">id</span><span class="sxs-lookup"><span data-stu-id="b9976-133">id</span></span>|<span data-ttu-id="b9976-134">String</span><span class="sxs-lookup"><span data-stu-id="b9976-134">String</span></span>|<span data-ttu-id="b9976-135">User experience analytics 指标历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b9976-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="b9976-136">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="b9976-136">metricDateTime</span></span>|<span data-ttu-id="b9976-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9976-137">DateTimeOffset</span></span>|<span data-ttu-id="b9976-138">User experience analytics 指标日期时间。</span><span class="sxs-lookup"><span data-stu-id="b9976-138">The user experience analytics metric date time.</span></span>|



## <a name="response"></a><span data-ttu-id="b9976-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9976-139">Response</span></span>
<span data-ttu-id="b9976-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9976-140">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9976-141">示例</span><span class="sxs-lookup"><span data-stu-id="b9976-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9976-142">请求</span><span class="sxs-lookup"><span data-stu-id="b9976-142">Request</span></span>
<span data-ttu-id="b9976-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9976-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b9976-144">响应</span><span class="sxs-lookup"><span data-stu-id="b9976-144">Response</span></span>
<span data-ttu-id="b9976-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9976-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 185

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```







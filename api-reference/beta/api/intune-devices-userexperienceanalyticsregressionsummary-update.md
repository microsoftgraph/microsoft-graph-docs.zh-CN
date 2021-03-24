---
title: 更新 userExperienceAnalyticsRegressionSummary
description: 更新 userExperienceAnalyticsRegressionSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2d2676d03751426a6524d28869300a185f7a4f9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146172"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="035b5-103">更新 userExperienceAnalyticsRegressionSummary</span><span class="sxs-lookup"><span data-stu-id="035b5-103">Update userExperienceAnalyticsRegressionSummary</span></span>

<span data-ttu-id="035b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="035b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="035b5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="035b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="035b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="035b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="035b5-107">更新 [userExperienceAnalyticsRegressionSummary 对象](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="035b5-107">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="035b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="035b5-108">Prerequisites</span></span>
<span data-ttu-id="035b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="035b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="035b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="035b5-111">Permission type</span></span>|<span data-ttu-id="035b5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="035b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="035b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="035b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="035b5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035b5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="035b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="035b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="035b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="035b5-116">Not supported.</span></span>|
|<span data-ttu-id="035b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="035b5-117">Application</span></span>|<span data-ttu-id="035b5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035b5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="035b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="035b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="035b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="035b5-120">Request headers</span></span>
|<span data-ttu-id="035b5-121">标头</span><span class="sxs-lookup"><span data-stu-id="035b5-121">Header</span></span>|<span data-ttu-id="035b5-122">值</span><span class="sxs-lookup"><span data-stu-id="035b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="035b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="035b5-123">Authorization</span></span>|<span data-ttu-id="035b5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="035b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="035b5-125">接受</span><span class="sxs-lookup"><span data-stu-id="035b5-125">Accept</span></span>|<span data-ttu-id="035b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="035b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="035b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="035b5-127">Request body</span></span>
<span data-ttu-id="035b5-128">在请求正文中，提供 [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="035b5-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="035b5-129">下表显示创建 [userExperienceAnalyticsRegressionSummary 时所需的属性](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="035b5-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="035b5-130">属性</span><span class="sxs-lookup"><span data-stu-id="035b5-130">Property</span></span>|<span data-ttu-id="035b5-131">类型</span><span class="sxs-lookup"><span data-stu-id="035b5-131">Type</span></span>|<span data-ttu-id="035b5-132">说明</span><span class="sxs-lookup"><span data-stu-id="035b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="035b5-133">id</span><span class="sxs-lookup"><span data-stu-id="035b5-133">id</span></span>|<span data-ttu-id="035b5-134">String</span><span class="sxs-lookup"><span data-stu-id="035b5-134">String</span></span>|<span data-ttu-id="035b5-135">用户体验分析回归摘要的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="035b5-135">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="035b5-136">响应</span><span class="sxs-lookup"><span data-stu-id="035b5-136">Response</span></span>
<span data-ttu-id="035b5-137">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="035b5-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="035b5-138">示例</span><span class="sxs-lookup"><span data-stu-id="035b5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="035b5-139">请求</span><span class="sxs-lookup"><span data-stu-id="035b5-139">Request</span></span>
<span data-ttu-id="035b5-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="035b5-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="035b5-141">响应</span><span class="sxs-lookup"><span data-stu-id="035b5-141">Response</span></span>
<span data-ttu-id="035b5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="035b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```





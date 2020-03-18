---
title: 更新 userExperienceAnalyticsRegressionSummary
description: 更新 userExperienceAnalyticsRegressionSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9fa85edbe35ec567557e82330d56cf042d258817
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813780"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="2c073-103">更新 userExperienceAnalyticsRegressionSummary</span><span class="sxs-lookup"><span data-stu-id="2c073-103">Update userExperienceAnalyticsRegressionSummary</span></span>

> <span data-ttu-id="2c073-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c073-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c073-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c073-106">更新[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c073-106">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c073-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c073-107">Prerequisites</span></span>
<span data-ttu-id="2c073-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c073-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c073-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c073-110">Permission type</span></span>|<span data-ttu-id="2c073-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c073-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c073-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c073-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c073-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c073-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2c073-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c073-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c073-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c073-115">Not supported.</span></span>|
|<span data-ttu-id="2c073-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c073-116">Application</span></span>|<span data-ttu-id="2c073-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c073-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c073-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c073-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="2c073-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c073-119">Request headers</span></span>
|<span data-ttu-id="2c073-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c073-120">Header</span></span>|<span data-ttu-id="2c073-121">值</span><span class="sxs-lookup"><span data-stu-id="2c073-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c073-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c073-122">Authorization</span></span>|<span data-ttu-id="2c073-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c073-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c073-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c073-124">Accept</span></span>|<span data-ttu-id="2c073-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c073-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c073-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c073-126">Request body</span></span>
<span data-ttu-id="2c073-127">在请求正文中，提供[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c073-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="2c073-128">下表显示创建[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c073-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="2c073-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c073-129">Property</span></span>|<span data-ttu-id="2c073-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c073-130">Type</span></span>|<span data-ttu-id="2c073-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c073-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c073-132">id</span><span class="sxs-lookup"><span data-stu-id="2c073-132">id</span></span>|<span data-ttu-id="2c073-133">String</span><span class="sxs-lookup"><span data-stu-id="2c073-133">String</span></span>|<span data-ttu-id="2c073-134">User experience analytics 回归摘要的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2c073-134">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="2c073-135">响应</span><span class="sxs-lookup"><span data-stu-id="2c073-135">Response</span></span>
<span data-ttu-id="2c073-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c073-136">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c073-137">示例</span><span class="sxs-lookup"><span data-stu-id="2c073-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c073-138">请求</span><span class="sxs-lookup"><span data-stu-id="2c073-138">Request</span></span>
<span data-ttu-id="2c073-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c073-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="2c073-140">响应</span><span class="sxs-lookup"><span data-stu-id="2c073-140">Response</span></span>
<span data-ttu-id="2c073-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c073-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```





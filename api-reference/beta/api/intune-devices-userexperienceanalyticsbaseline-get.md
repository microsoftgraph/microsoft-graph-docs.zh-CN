---
title: 获取 userExperienceAnalyticsBaseline
description: 读取 userExperienceAnalyticsBaseline 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3463cdbf13fb758a344c372797f6e7990acb9b1b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773257"
---
# <a name="get-userexperienceanalyticsbaseline"></a><span data-ttu-id="69400-103">获取 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="69400-103">Get userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="69400-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69400-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69400-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69400-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69400-106">读取[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69400-106">Read properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69400-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69400-107">Prerequisites</span></span>
<span data-ttu-id="69400-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69400-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69400-110">Permission type</span></span>|<span data-ttu-id="69400-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69400-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69400-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69400-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69400-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69400-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="69400-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69400-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69400-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69400-115">Not supported.</span></span>|
|<span data-ttu-id="69400-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69400-116">Application</span></span>|<span data-ttu-id="69400-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69400-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69400-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69400-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69400-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69400-119">Optional query parameters</span></span>
<span data-ttu-id="69400-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69400-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69400-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="69400-121">Request headers</span></span>
|<span data-ttu-id="69400-122">标头</span><span class="sxs-lookup"><span data-stu-id="69400-122">Header</span></span>|<span data-ttu-id="69400-123">值</span><span class="sxs-lookup"><span data-stu-id="69400-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69400-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69400-124">Authorization</span></span>|<span data-ttu-id="69400-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69400-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69400-126">接受</span><span class="sxs-lookup"><span data-stu-id="69400-126">Accept</span></span>|<span data-ttu-id="69400-127">application/json</span><span class="sxs-lookup"><span data-stu-id="69400-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69400-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="69400-128">Request body</span></span>
<span data-ttu-id="69400-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69400-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69400-130">响应</span><span class="sxs-lookup"><span data-stu-id="69400-130">Response</span></span>
<span data-ttu-id="69400-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69400-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69400-132">示例</span><span class="sxs-lookup"><span data-stu-id="69400-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="69400-133">请求</span><span class="sxs-lookup"><span data-stu-id="69400-133">Request</span></span>
<span data-ttu-id="69400-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69400-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

### <a name="response"></a><span data-ttu-id="69400-135">响应</span><span class="sxs-lookup"><span data-stu-id="69400-135">Response</span></span>
<span data-ttu-id="69400-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69400-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
    "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
    "displayName": "Display Name value",
    "overallScore": 12,
    "isBuiltIn": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
  }
}
```





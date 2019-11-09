---
title: 获取 deviceManagementIntentSettingCategory
description: 读取 deviceManagementIntentSettingCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3881c6c1991d40cf77e86475b737492843e4f32
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087725"
---
# <a name="get-devicemanagementintentsettingcategory"></a><span data-ttu-id="db618-103">获取 deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="db618-103">Get deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="db618-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db618-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db618-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db618-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db618-106">读取[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db618-106">Read properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db618-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db618-107">Prerequisites</span></span>
<span data-ttu-id="db618-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db618-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db618-110">Permission type</span></span>|<span data-ttu-id="db618-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db618-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db618-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db618-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db618-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db618-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db618-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db618-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db618-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db618-115">Not supported.</span></span>|
|<span data-ttu-id="db618-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db618-116">Application</span></span>|<span data-ttu-id="db618-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db618-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db618-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db618-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db618-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db618-119">Optional query parameters</span></span>
<span data-ttu-id="db618-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db618-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db618-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="db618-121">Request headers</span></span>
|<span data-ttu-id="db618-122">标头</span><span class="sxs-lookup"><span data-stu-id="db618-122">Header</span></span>|<span data-ttu-id="db618-123">值</span><span class="sxs-lookup"><span data-stu-id="db618-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db618-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="db618-124">Authorization</span></span>|<span data-ttu-id="db618-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db618-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db618-126">接受</span><span class="sxs-lookup"><span data-stu-id="db618-126">Accept</span></span>|<span data-ttu-id="db618-127">application/json</span><span class="sxs-lookup"><span data-stu-id="db618-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db618-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db618-128">Request body</span></span>
<span data-ttu-id="db618-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db618-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db618-130">响应</span><span class="sxs-lookup"><span data-stu-id="db618-130">Response</span></span>
<span data-ttu-id="db618-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="db618-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db618-132">示例</span><span class="sxs-lookup"><span data-stu-id="db618-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="db618-133">请求</span><span class="sxs-lookup"><span data-stu-id="db618-133">Request</span></span>
<span data-ttu-id="db618-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db618-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="db618-135">响应</span><span class="sxs-lookup"><span data-stu-id="db618-135">Response</span></span>
<span data-ttu-id="db618-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db618-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
    "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
    "displayName": "Display Name value"
  }
}
```







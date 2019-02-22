---
title: 获取 mobileAppCategory
description: 读取 mobileAppCategory 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 259874e721b995649a2b030a9e923869cc431717
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153632"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="21c99-103">获取 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="21c99-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="21c99-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21c99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21c99-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21c99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21c99-106">读取 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21c99-106">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21c99-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="21c99-107">Prerequisites</span></span>
<span data-ttu-id="21c99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="21c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21c99-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="21c99-110">Permission type</span></span>|<span data-ttu-id="21c99-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21c99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21c99-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21c99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21c99-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21c99-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21c99-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21c99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21c99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="21c99-115">Not supported.</span></span>|
|<span data-ttu-id="21c99-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="21c99-116">Application</span></span>|<span data-ttu-id="21c99-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="21c99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21c99-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21c99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21c99-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="21c99-119">Optional query parameters</span></span>
<span data-ttu-id="21c99-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="21c99-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21c99-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="21c99-121">Request headers</span></span>
|<span data-ttu-id="21c99-122">标头</span><span class="sxs-lookup"><span data-stu-id="21c99-122">Header</span></span>|<span data-ttu-id="21c99-123">值</span><span class="sxs-lookup"><span data-stu-id="21c99-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21c99-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="21c99-124">Authorization</span></span>|<span data-ttu-id="21c99-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21c99-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21c99-126">Accept</span><span class="sxs-lookup"><span data-stu-id="21c99-126">Accept</span></span>|<span data-ttu-id="21c99-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21c99-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21c99-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="21c99-128">Request body</span></span>
<span data-ttu-id="21c99-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21c99-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21c99-130">响应</span><span class="sxs-lookup"><span data-stu-id="21c99-130">Response</span></span>
<span data-ttu-id="21c99-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21c99-131">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21c99-132">示例</span><span class="sxs-lookup"><span data-stu-id="21c99-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="21c99-133">请求</span><span class="sxs-lookup"><span data-stu-id="21c99-133">Request</span></span>
<span data-ttu-id="21c99-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21c99-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="21c99-135">响应</span><span class="sxs-lookup"><span data-stu-id="21c99-135">Response</span></span>
<span data-ttu-id="21c99-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21c99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





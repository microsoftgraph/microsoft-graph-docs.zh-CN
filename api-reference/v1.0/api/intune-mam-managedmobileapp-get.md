---
title: 获取 managedMobileApp
description: 读取 managedMobileApp 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbbc301310cc5986b1bbdbd488d346d894526272
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363400"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="cf0ab-103">获取 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="cf0ab-103">Get managedMobileApp</span></span>

> <span data-ttu-id="cf0ab-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf0ab-105">读取 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-105">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf0ab-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf0ab-106">Prerequisites</span></span>
<span data-ttu-id="cf0ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf0ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf0ab-109">Permission type</span></span>|<span data-ttu-id="cf0ab-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf0ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf0ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf0ab-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf0ab-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf0ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf0ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-114">Not supported.</span></span>|
|<span data-ttu-id="cf0ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf0ab-115">Application</span></span>|<span data-ttu-id="cf0ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf0ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf0ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf0ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf0ab-118">Optional query parameters</span></span>
<span data-ttu-id="cf0ab-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf0ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf0ab-120">Request headers</span></span>
|<span data-ttu-id="cf0ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="cf0ab-121">Header</span></span>|<span data-ttu-id="cf0ab-122">值</span><span class="sxs-lookup"><span data-stu-id="cf0ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf0ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf0ab-123">Authorization</span></span>|<span data-ttu-id="cf0ab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf0ab-125">接受</span><span class="sxs-lookup"><span data-stu-id="cf0ab-125">Accept</span></span>|<span data-ttu-id="cf0ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf0ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf0ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf0ab-127">Request body</span></span>
<span data-ttu-id="cf0ab-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf0ab-129">响应</span><span class="sxs-lookup"><span data-stu-id="cf0ab-129">Response</span></span>
<span data-ttu-id="cf0ab-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-130">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf0ab-131">示例</span><span class="sxs-lookup"><span data-stu-id="cf0ab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf0ab-132">请求</span><span class="sxs-lookup"><span data-stu-id="cf0ab-132">Request</span></span>
<span data-ttu-id="cf0ab-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="cf0ab-134">响应</span><span class="sxs-lookup"><span data-stu-id="cf0ab-134">Response</span></span>
<span data-ttu-id="cf0ab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf0ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```





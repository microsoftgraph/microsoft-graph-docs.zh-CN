---
title: 获取 managedIOSStoreApp
description: 读取 managedIOSStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69693bcf1a51916af6f7d2e0f42930709aa76e6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442511"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="31834-103">获取 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="31834-103">Get managedIOSStoreApp</span></span>

<span data-ttu-id="31834-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31834-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31834-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31834-106">读取 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31834-106">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31834-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="31834-107">Prerequisites</span></span>
<span data-ttu-id="31834-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="31834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31834-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="31834-110">Permission type</span></span>|<span data-ttu-id="31834-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31834-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31834-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31834-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31834-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31834-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="31834-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31834-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31834-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31834-115">Not supported.</span></span>|
|<span data-ttu-id="31834-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="31834-116">Application</span></span>|<span data-ttu-id="31834-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31834-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31834-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31834-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31834-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31834-119">Optional query parameters</span></span>
<span data-ttu-id="31834-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31834-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31834-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="31834-121">Request headers</span></span>
|<span data-ttu-id="31834-122">标头</span><span class="sxs-lookup"><span data-stu-id="31834-122">Header</span></span>|<span data-ttu-id="31834-123">值</span><span class="sxs-lookup"><span data-stu-id="31834-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31834-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="31834-124">Authorization</span></span>|<span data-ttu-id="31834-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31834-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31834-126">接受</span><span class="sxs-lookup"><span data-stu-id="31834-126">Accept</span></span>|<span data-ttu-id="31834-127">application/json</span><span class="sxs-lookup"><span data-stu-id="31834-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31834-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="31834-128">Request body</span></span>
<span data-ttu-id="31834-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31834-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31834-130">响应</span><span class="sxs-lookup"><span data-stu-id="31834-130">Response</span></span>
<span data-ttu-id="31834-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31834-131">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31834-132">示例</span><span class="sxs-lookup"><span data-stu-id="31834-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="31834-133">请求</span><span class="sxs-lookup"><span data-stu-id="31834-133">Request</span></span>
<span data-ttu-id="31834-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31834-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="31834-135">响应</span><span class="sxs-lookup"><span data-stu-id="31834-135">Response</span></span>
<span data-ttu-id="31834-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31834-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1369

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSStoreApp",
    "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "bundleId": "Bundle Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true,
      "v13_0": true
    }
  }
}
```







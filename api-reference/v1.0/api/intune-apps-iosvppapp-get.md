---
title: 获取 iosVppApp
description: 读取 iosVppApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9841c1ac70735e1dc9291b812d8fd268f1c2b30
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456162"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="17ea8-103">获取 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="17ea8-103">Get iosVppApp</span></span>

<span data-ttu-id="17ea8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17ea8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17ea8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17ea8-106">读取 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17ea8-106">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17ea8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="17ea8-107">Prerequisites</span></span>
<span data-ttu-id="17ea8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17ea8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="17ea8-110">Permission type</span></span>|<span data-ttu-id="17ea8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17ea8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ea8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17ea8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17ea8-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="17ea8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="17ea8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17ea8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ea8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17ea8-115">Not supported.</span></span>|
|<span data-ttu-id="17ea8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="17ea8-116">Application</span></span>|<span data-ttu-id="17ea8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="17ea8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ea8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17ea8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17ea8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17ea8-119">Optional query parameters</span></span>
<span data-ttu-id="17ea8-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17ea8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17ea8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="17ea8-121">Request headers</span></span>
|<span data-ttu-id="17ea8-122">标头</span><span class="sxs-lookup"><span data-stu-id="17ea8-122">Header</span></span>|<span data-ttu-id="17ea8-123">值</span><span class="sxs-lookup"><span data-stu-id="17ea8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ea8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="17ea8-124">Authorization</span></span>|<span data-ttu-id="17ea8-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17ea8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17ea8-126">接受</span><span class="sxs-lookup"><span data-stu-id="17ea8-126">Accept</span></span>|<span data-ttu-id="17ea8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17ea8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ea8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="17ea8-128">Request body</span></span>
<span data-ttu-id="17ea8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17ea8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17ea8-130">响应</span><span class="sxs-lookup"><span data-stu-id="17ea8-130">Response</span></span>
<span data-ttu-id="17ea8-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17ea8-131">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ea8-132">示例</span><span class="sxs-lookup"><span data-stu-id="17ea8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17ea8-133">请求</span><span class="sxs-lookup"><span data-stu-id="17ea8-133">Request</span></span>
<span data-ttu-id="17ea8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17ea8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="17ea8-135">响应</span><span class="sxs-lookup"><span data-stu-id="17ea8-135">Response</span></span>
<span data-ttu-id="17ea8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17ea8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value"
  }
}
```







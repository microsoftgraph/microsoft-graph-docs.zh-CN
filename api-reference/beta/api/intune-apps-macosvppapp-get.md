---
title: 获取 macOsVppApp
description: 读取 macOsVppApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0c69e58f34d69d92a1693cce60fed3028db1025
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143820"
---
# <a name="get-macosvppapp"></a><span data-ttu-id="cb3f1-103">获取 macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="cb3f1-103">Get macOsVppApp</span></span>

<span data-ttu-id="cb3f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb3f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb3f1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb3f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb3f1-107">读取 [macOsVppApp 对象的属性和](../resources/intune-apps-macosvppapp.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-107">Read properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb3f1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb3f1-108">Prerequisites</span></span>
<span data-ttu-id="cb3f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb3f1-111">Permission type</span></span>|<span data-ttu-id="cb3f1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb3f1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb3f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb3f1-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3f1-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb3f1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb3f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-116">Not supported.</span></span>|
|<span data-ttu-id="cb3f1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb3f1-117">Application</span></span>|<span data-ttu-id="cb3f1-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3f1-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3f1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb3f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb3f1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb3f1-120">Optional query parameters</span></span>
<span data-ttu-id="cb3f1-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb3f1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb3f1-122">Request headers</span></span>
|<span data-ttu-id="cb3f1-123">标头</span><span class="sxs-lookup"><span data-stu-id="cb3f1-123">Header</span></span>|<span data-ttu-id="cb3f1-124">值</span><span class="sxs-lookup"><span data-stu-id="cb3f1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3f1-125">Authorization</span></span>|<span data-ttu-id="cb3f1-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3f1-127">接受</span><span class="sxs-lookup"><span data-stu-id="cb3f1-127">Accept</span></span>|<span data-ttu-id="cb3f1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3f1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3f1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb3f1-129">Request body</span></span>
<span data-ttu-id="cb3f1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3f1-131">响应</span><span class="sxs-lookup"><span data-stu-id="cb3f1-131">Response</span></span>
<span data-ttu-id="cb3f1-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [macOsVppApp](../resources/intune-apps-macosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-132">If successful, this method returns a `200 OK` response code and [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3f1-133">示例</span><span class="sxs-lookup"><span data-stu-id="cb3f1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb3f1-134">请求</span><span class="sxs-lookup"><span data-stu-id="cb3f1-134">Request</span></span>
<span data-ttu-id="cb3f1-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="cb3f1-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb3f1-136">Response</span></span>
<span data-ttu-id="cb3f1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb3f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2231

{
  "value": {
    "@odata.type": "#microsoft.graph.macOsVppApp",
    "id": "10b95265-5265-10b9-6552-b9106552b910",
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
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value",
    "vppTokenId": "Vpp Token Id value",
    "revokeLicenseActionResults": [
      {
        "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
        "userId": "User Id value",
        "managedDeviceId": "Managed Device Id value",
        "totalLicensesCount": 2,
        "failedLicensesCount": 3,
        "actionFailureReason": "appleFailure",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ]
  }
}
```





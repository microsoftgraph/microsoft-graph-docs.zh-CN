---
title: 列出 iosVppApps
description: 列出 iosVppApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6b87c10ad86fe7bfe912c8f8e800823661f2381
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987027"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="707a0-103">列出 iosVppApps</span><span class="sxs-lookup"><span data-stu-id="707a0-103">List iosVppApps</span></span>

<span data-ttu-id="707a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="707a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="707a0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="707a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="707a0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="707a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="707a0-107">列出 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="707a0-107">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="707a0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="707a0-108">Prerequisites</span></span>
<span data-ttu-id="707a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="707a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="707a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="707a0-111">Permission type</span></span>|<span data-ttu-id="707a0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="707a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="707a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="707a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="707a0-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="707a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="707a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="707a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="707a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="707a0-116">Not supported.</span></span>|
|<span data-ttu-id="707a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="707a0-117">Application</span></span>|<span data-ttu-id="707a0-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="707a0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="707a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="707a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="707a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="707a0-120">Request headers</span></span>
|<span data-ttu-id="707a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="707a0-121">Header</span></span>|<span data-ttu-id="707a0-122">值</span><span class="sxs-lookup"><span data-stu-id="707a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="707a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="707a0-123">Authorization</span></span>|<span data-ttu-id="707a0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="707a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="707a0-125">接受</span><span class="sxs-lookup"><span data-stu-id="707a0-125">Accept</span></span>|<span data-ttu-id="707a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="707a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="707a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="707a0-127">Request body</span></span>
<span data-ttu-id="707a0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="707a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="707a0-129">响应</span><span class="sxs-lookup"><span data-stu-id="707a0-129">Response</span></span>
<span data-ttu-id="707a0-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="707a0-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="707a0-131">示例</span><span class="sxs-lookup"><span data-stu-id="707a0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="707a0-132">请求</span><span class="sxs-lookup"><span data-stu-id="707a0-132">Request</span></span>
<span data-ttu-id="707a0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="707a0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="707a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="707a0-134">Response</span></span>
<span data-ttu-id="707a0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="707a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2509

{
  "value": [
    {
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
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
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
  ]
}
```







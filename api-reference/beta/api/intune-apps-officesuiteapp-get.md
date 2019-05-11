---
title: 获取 officeSuiteApp
description: 读取 officeSuiteApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ad4fda6cd51d84c5e005b0dbcde5d557873f87c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934969"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="da8c2-103">获取 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="da8c2-103">Get officeSuiteApp</span></span>

> <span data-ttu-id="da8c2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da8c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da8c2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da8c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da8c2-106">读取[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da8c2-106">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da8c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da8c2-107">Prerequisites</span></span>
<span data-ttu-id="da8c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da8c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da8c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da8c2-110">Permission type</span></span>|<span data-ttu-id="da8c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da8c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da8c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da8c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da8c2-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da8c2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da8c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da8c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da8c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da8c2-115">Not supported.</span></span>|
|<span data-ttu-id="da8c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da8c2-116">Application</span></span>|<span data-ttu-id="da8c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da8c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da8c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da8c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da8c2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da8c2-119">Optional query parameters</span></span>
<span data-ttu-id="da8c2-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da8c2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da8c2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="da8c2-121">Request headers</span></span>
|<span data-ttu-id="da8c2-122">标头</span><span class="sxs-lookup"><span data-stu-id="da8c2-122">Header</span></span>|<span data-ttu-id="da8c2-123">值</span><span class="sxs-lookup"><span data-stu-id="da8c2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da8c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da8c2-124">Authorization</span></span>|<span data-ttu-id="da8c2-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da8c2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da8c2-126">接受</span><span class="sxs-lookup"><span data-stu-id="da8c2-126">Accept</span></span>|<span data-ttu-id="da8c2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="da8c2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da8c2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="da8c2-128">Request body</span></span>
<span data-ttu-id="da8c2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da8c2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da8c2-130">响应</span><span class="sxs-lookup"><span data-stu-id="da8c2-130">Response</span></span>
<span data-ttu-id="da8c2-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da8c2-131">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da8c2-132">示例</span><span class="sxs-lookup"><span data-stu-id="da8c2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="da8c2-133">请求</span><span class="sxs-lookup"><span data-stu-id="da8c2-133">Request</span></span>
<span data-ttu-id="da8c2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da8c2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="da8c2-135">响应</span><span class="sxs-lookup"><span data-stu-id="da8c2-135">Response</span></span>
<span data-ttu-id="da8c2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da8c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1904

{
  "value": {
    "@odata.type": "#microsoft.graph.officeSuiteApp",
    "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
    "autoAcceptEula": true,
    "productIds": [
      "o365BusinessRetail"
    ],
    "excludedApps": {
      "@odata.type": "microsoft.graph.excludedApps",
      "access": true,
      "excel": true,
      "groove": true,
      "infoPath": true,
      "lync": true,
      "oneDrive": true,
      "oneNote": true,
      "outlook": true,
      "powerPoint": true,
      "publisher": true,
      "sharePointDesigner": true,
      "teams": true,
      "visio": true,
      "word": true
    },
    "useSharedComputerActivation": true,
    "updateChannel": "current",
    "officePlatformArchitecture": "x86",
    "localesToInstall": [
      "Locales To Install value"
    ],
    "installProgressDisplayLevel": "full",
    "shouldUninstallOlderVersionsOfOffice": true,
    "targetVersion": "Target Version value",
    "updateVersion": "Update Version value",
    "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
  }
}
```





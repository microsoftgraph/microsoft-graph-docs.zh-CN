---
title: 获取 androidForWorkApp
description: 读取 androidForWorkApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e29e7d0914b4ae96d62881231e84c1d4e51586ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012458"
---
# <a name="get-androidforworkapp"></a><span data-ttu-id="ffe05-103">获取 androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="ffe05-103">Get androidForWorkApp</span></span>

<span data-ttu-id="ffe05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffe05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffe05-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffe05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffe05-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffe05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffe05-107">读取 [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffe05-107">Read properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffe05-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffe05-108">Prerequisites</span></span>
<span data-ttu-id="ffe05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffe05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffe05-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffe05-111">Permission type</span></span>|<span data-ttu-id="ffe05-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffe05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffe05-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffe05-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffe05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ffe05-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffe05-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffe05-116">Not supported.</span></span>|
|<span data-ttu-id="ffe05-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffe05-117">Application</span></span>|<span data-ttu-id="ffe05-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffe05-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffe05-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffe05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffe05-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ffe05-120">Optional query parameters</span></span>
<span data-ttu-id="ffe05-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ffe05-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffe05-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffe05-122">Request headers</span></span>
|<span data-ttu-id="ffe05-123">标头</span><span class="sxs-lookup"><span data-stu-id="ffe05-123">Header</span></span>|<span data-ttu-id="ffe05-124">值</span><span class="sxs-lookup"><span data-stu-id="ffe05-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffe05-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe05-125">Authorization</span></span>|<span data-ttu-id="ffe05-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffe05-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffe05-127">接受</span><span class="sxs-lookup"><span data-stu-id="ffe05-127">Accept</span></span>|<span data-ttu-id="ffe05-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe05-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffe05-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffe05-129">Request body</span></span>
<span data-ttu-id="ffe05-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffe05-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffe05-131">响应</span><span class="sxs-lookup"><span data-stu-id="ffe05-131">Response</span></span>
<span data-ttu-id="ffe05-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe05-132">If successful, this method returns a `200 OK` response code and [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe05-133">示例</span><span class="sxs-lookup"><span data-stu-id="ffe05-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffe05-134">请求</span><span class="sxs-lookup"><span data-stu-id="ffe05-134">Request</span></span>
<span data-ttu-id="ffe05-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffe05-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ffe05-136">响应</span><span class="sxs-lookup"><span data-stu-id="ffe05-136">Response</span></span>
<span data-ttu-id="ffe05-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffe05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1215

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkApp",
    "id": "c5010785-0785-c501-8507-01c5850701c5",
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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```







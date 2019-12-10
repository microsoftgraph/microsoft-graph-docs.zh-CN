---
title: 获取了 windowsphone81appx
description: 读取了 windowsphone81appx 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 566b2881623d25653db0fa1e77fa93480733f893
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933305"
---
# <a name="get-windowsphone81appx"></a><span data-ttu-id="7d527-103">获取了 windowsphone81appx</span><span class="sxs-lookup"><span data-stu-id="7d527-103">Get windowsPhone81AppX</span></span>

> <span data-ttu-id="7d527-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d527-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d527-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d527-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d527-106">读取[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d527-106">Read properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d527-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d527-107">Prerequisites</span></span>
<span data-ttu-id="7d527-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d527-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d527-110">Permission type</span></span>|<span data-ttu-id="7d527-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d527-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d527-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d527-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d527-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d527-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d527-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d527-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d527-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d527-115">Not supported.</span></span>|
|<span data-ttu-id="7d527-116">Application</span><span class="sxs-lookup"><span data-stu-id="7d527-116">Application</span></span>|<span data-ttu-id="7d527-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d527-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d527-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d527-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d527-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7d527-119">Optional query parameters</span></span>
<span data-ttu-id="7d527-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7d527-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d527-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d527-121">Request headers</span></span>
|<span data-ttu-id="7d527-122">标头</span><span class="sxs-lookup"><span data-stu-id="7d527-122">Header</span></span>|<span data-ttu-id="7d527-123">值</span><span class="sxs-lookup"><span data-stu-id="7d527-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d527-124">授权</span><span class="sxs-lookup"><span data-stu-id="7d527-124">Authorization</span></span>|<span data-ttu-id="7d527-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d527-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d527-126">接受</span><span class="sxs-lookup"><span data-stu-id="7d527-126">Accept</span></span>|<span data-ttu-id="7d527-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7d527-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d527-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d527-128">Request body</span></span>
<span data-ttu-id="7d527-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d527-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d527-130">响应</span><span class="sxs-lookup"><span data-stu-id="7d527-130">Response</span></span>
<span data-ttu-id="7d527-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7d527-131">If successful, this method returns a `200 OK` response code and [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d527-132">示例</span><span class="sxs-lookup"><span data-stu-id="7d527-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d527-133">请求</span><span class="sxs-lookup"><span data-stu-id="7d527-133">Request</span></span>
<span data-ttu-id="7d527-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d527-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7d527-135">响应</span><span class="sxs-lookup"><span data-stu-id="7d527-135">Response</span></span>
<span data-ttu-id="7d527-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d527-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1798

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppX",
    "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true
    },
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value"
  }
}
```






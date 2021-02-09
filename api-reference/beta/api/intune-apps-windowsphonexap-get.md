---
title: 获取 windowsPhoneXAP
description: 读取 windowsPhoneXAP 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d8a7b8f5235abd9a0610524279cb278e4490a25
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155305"
---
# <a name="get-windowsphonexap"></a><span data-ttu-id="566ec-103">获取 windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="566ec-103">Get windowsPhoneXAP</span></span>

<span data-ttu-id="566ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="566ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="566ec-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="566ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="566ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="566ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="566ec-107">读取 [windowsPhoneXAP 对象的属性和](../resources/intune-apps-windowsphonexap.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="566ec-107">Read properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="566ec-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="566ec-108">Prerequisites</span></span>
<span data-ttu-id="566ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="566ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="566ec-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="566ec-111">Permission type</span></span>|<span data-ttu-id="566ec-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="566ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="566ec-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="566ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="566ec-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="566ec-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="566ec-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="566ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="566ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="566ec-116">Not supported.</span></span>|
|<span data-ttu-id="566ec-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="566ec-117">Application</span></span>|<span data-ttu-id="566ec-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="566ec-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="566ec-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="566ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="566ec-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="566ec-120">Optional query parameters</span></span>
<span data-ttu-id="566ec-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="566ec-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="566ec-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="566ec-122">Request headers</span></span>
|<span data-ttu-id="566ec-123">标头</span><span class="sxs-lookup"><span data-stu-id="566ec-123">Header</span></span>|<span data-ttu-id="566ec-124">值</span><span class="sxs-lookup"><span data-stu-id="566ec-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="566ec-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="566ec-125">Authorization</span></span>|<span data-ttu-id="566ec-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="566ec-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="566ec-127">接受</span><span class="sxs-lookup"><span data-stu-id="566ec-127">Accept</span></span>|<span data-ttu-id="566ec-128">application/json</span><span class="sxs-lookup"><span data-stu-id="566ec-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="566ec-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="566ec-129">Request body</span></span>
<span data-ttu-id="566ec-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="566ec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="566ec-131">响应</span><span class="sxs-lookup"><span data-stu-id="566ec-131">Response</span></span>
<span data-ttu-id="566ec-132">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="566ec-132">If successful, this method returns a `200 OK` response code and [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="566ec-133">示例</span><span class="sxs-lookup"><span data-stu-id="566ec-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="566ec-134">请求</span><span class="sxs-lookup"><span data-stu-id="566ec-134">Request</span></span>
<span data-ttu-id="566ec-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="566ec-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="566ec-136">响应</span><span class="sxs-lookup"><span data-stu-id="566ec-136">Response</span></span>
<span data-ttu-id="566ec-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="566ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1623

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhoneXAP",
    "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
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
      "v10_1903": true,
      "v10_1909": true,
      "v10_2004": true
    },
    "productIdentifier": "Product Identifier value",
    "identityVersion": "Identity Version value"
  }
}
```





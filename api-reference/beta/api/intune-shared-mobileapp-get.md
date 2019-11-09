---
title: 获取 mobileApp
description: 读取 mobileApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6390772c1d9e275387023569cf24e5396d0dc1dd
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085799"
---
# <a name="get-mobileapp"></a><span data-ttu-id="cb865-103">获取 mobileApp</span><span class="sxs-lookup"><span data-stu-id="cb865-103">Get mobileApp</span></span>

> <span data-ttu-id="cb865-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb865-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb865-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb865-106">读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb865-106">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb865-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb865-107">Prerequisites</span></span>
<span data-ttu-id="cb865-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb865-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb865-110">Permission type</span></span>|<span data-ttu-id="cb865-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb865-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb865-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb865-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cb865-113">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="cb865-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="cb865-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb865-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="cb865-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="cb865-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cb865-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb865-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cb865-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb865-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb865-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb865-118">Not supported.</span></span>|
|<span data-ttu-id="cb865-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb865-119">Application</span></span>||
| <span data-ttu-id="cb865-120">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="cb865-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="cb865-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb865-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="cb865-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="cb865-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cb865-123">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb865-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb865-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb865-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb865-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb865-125">Optional query parameters</span></span>
<span data-ttu-id="cb865-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb865-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb865-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb865-127">Request headers</span></span>
|<span data-ttu-id="cb865-128">标头</span><span class="sxs-lookup"><span data-stu-id="cb865-128">Header</span></span>|<span data-ttu-id="cb865-129">值</span><span class="sxs-lookup"><span data-stu-id="cb865-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb865-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb865-130">Authorization</span></span>|<span data-ttu-id="cb865-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb865-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb865-132">接受</span><span class="sxs-lookup"><span data-stu-id="cb865-132">Accept</span></span>|<span data-ttu-id="cb865-133">application/json</span><span class="sxs-lookup"><span data-stu-id="cb865-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb865-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb865-134">Request body</span></span>
<span data-ttu-id="cb865-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb865-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb865-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb865-136">Response</span></span>
<span data-ttu-id="cb865-137">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [mobileApp](../resources/intune-shared-mobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb865-137">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-shared-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb865-138">示例</span><span class="sxs-lookup"><span data-stu-id="cb865-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb865-139">请求</span><span class="sxs-lookup"><span data-stu-id="cb865-139">Request</span></span>
<span data-ttu-id="cb865-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb865-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="cb865-141">响应</span><span class="sxs-lookup"><span data-stu-id="cb865-141">Response</span></span>
<span data-ttu-id="cb865-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb865-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 949

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileApp",
    "id": "0177548a-548a-0177-8a54-77018a547701",
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
    "dependentAppCount": 1
  }
}
```










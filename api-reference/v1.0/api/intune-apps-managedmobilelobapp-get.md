---
title: 获取 managedMobileLobApp
description: 读取 managedMobileLobApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a05a6f18687563a4a28c213376971ea0b8ad9703
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070077"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="f7aca-103">获取 managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="f7aca-103">Get managedMobileLobApp</span></span>

<span data-ttu-id="f7aca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7aca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7aca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7aca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7aca-106">读取 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7aca-106">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7aca-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7aca-107">Prerequisites</span></span>
<span data-ttu-id="f7aca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7aca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7aca-110">Permission type</span></span>|<span data-ttu-id="f7aca-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7aca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7aca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7aca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7aca-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7aca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7aca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7aca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7aca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7aca-115">Not supported.</span></span>|
|<span data-ttu-id="f7aca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7aca-116">Application</span></span>|<span data-ttu-id="f7aca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7aca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7aca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7aca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7aca-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7aca-119">Optional query parameters</span></span>
<span data-ttu-id="f7aca-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7aca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7aca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7aca-121">Request headers</span></span>
|<span data-ttu-id="f7aca-122">标头</span><span class="sxs-lookup"><span data-stu-id="f7aca-122">Header</span></span>|<span data-ttu-id="f7aca-123">值</span><span class="sxs-lookup"><span data-stu-id="f7aca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7aca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7aca-124">Authorization</span></span>|<span data-ttu-id="f7aca-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7aca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7aca-126">接受</span><span class="sxs-lookup"><span data-stu-id="f7aca-126">Accept</span></span>|<span data-ttu-id="f7aca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7aca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7aca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7aca-128">Request body</span></span>
<span data-ttu-id="f7aca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7aca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7aca-130">响应</span><span class="sxs-lookup"><span data-stu-id="f7aca-130">Response</span></span>
<span data-ttu-id="f7aca-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7aca-131">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7aca-132">示例</span><span class="sxs-lookup"><span data-stu-id="f7aca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7aca-133">请求</span><span class="sxs-lookup"><span data-stu-id="f7aca-133">Request</span></span>
<span data-ttu-id="f7aca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7aca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f7aca-135">响应</span><span class="sxs-lookup"><span data-stu-id="f7aca-135">Response</span></span>
<span data-ttu-id="f7aca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```










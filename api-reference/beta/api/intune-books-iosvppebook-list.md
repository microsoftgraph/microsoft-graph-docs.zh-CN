---
title: 列出 iosVppEBooks
description: 列出 iosVppEBook 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a2496cdaeff31a9e2b9c8f587eb317ed0a49edba
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716178"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="24d0e-103">列出 iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="24d0e-103">List iosVppEBooks</span></span>

<span data-ttu-id="24d0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24d0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24d0e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24d0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24d0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24d0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24d0e-107">列出 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24d0e-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24d0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24d0e-108">Prerequisites</span></span>
<span data-ttu-id="24d0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24d0e-111">Permission type</span></span>|<span data-ttu-id="24d0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24d0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24d0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24d0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24d0e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24d0e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="24d0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24d0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24d0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24d0e-116">Not supported.</span></span>|
|<span data-ttu-id="24d0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="24d0e-117">Application</span></span>|<span data-ttu-id="24d0e-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24d0e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24d0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24d0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="24d0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24d0e-120">Request headers</span></span>
|<span data-ttu-id="24d0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="24d0e-121">Header</span></span>|<span data-ttu-id="24d0e-122">值</span><span class="sxs-lookup"><span data-stu-id="24d0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24d0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d0e-123">Authorization</span></span>|<span data-ttu-id="24d0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24d0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24d0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="24d0e-125">Accept</span></span>|<span data-ttu-id="24d0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24d0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24d0e-127">Request body</span></span>
<span data-ttu-id="24d0e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24d0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24d0e-129">响应</span><span class="sxs-lookup"><span data-stu-id="24d0e-129">Response</span></span>
<span data-ttu-id="24d0e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="24d0e-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="24d0e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24d0e-132">请求</span><span class="sxs-lookup"><span data-stu-id="24d0e-132">Request</span></span>
<span data-ttu-id="24d0e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24d0e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="24d0e-134">响应</span><span class="sxs-lookup"><span data-stu-id="24d0e-134">Response</span></span>
<span data-ttu-id="24d0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24d0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






---
title: 列出 iosVppEBooks
description: 列出 iosVppEBook 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 942a00f848ee5770b6b720513c1f55f3408c7a65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32484270"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="c1e97-103">列出 iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="c1e97-103">List iosVppEBooks</span></span>

> <span data-ttu-id="c1e97-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1e97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1e97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1e97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1e97-106">列出 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1e97-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1e97-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1e97-107">Prerequisites</span></span>
<span data-ttu-id="c1e97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1e97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1e97-110">Permission type</span></span>|<span data-ttu-id="c1e97-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1e97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1e97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1e97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1e97-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1e97-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1e97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1e97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1e97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1e97-115">Not supported.</span></span>|
|<span data-ttu-id="c1e97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1e97-116">Application</span></span>|<span data-ttu-id="c1e97-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1e97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1e97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1e97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c1e97-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1e97-119">Request headers</span></span>
|<span data-ttu-id="c1e97-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1e97-120">Header</span></span>|<span data-ttu-id="c1e97-121">值</span><span class="sxs-lookup"><span data-stu-id="c1e97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1e97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1e97-122">Authorization</span></span>|<span data-ttu-id="c1e97-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1e97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1e97-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1e97-124">Accept</span></span>|<span data-ttu-id="c1e97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1e97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1e97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1e97-126">Request body</span></span>
<span data-ttu-id="c1e97-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1e97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1e97-128">响应</span><span class="sxs-lookup"><span data-stu-id="c1e97-128">Response</span></span>
<span data-ttu-id="c1e97-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1e97-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1e97-130">示例</span><span class="sxs-lookup"><span data-stu-id="c1e97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1e97-131">请求</span><span class="sxs-lookup"><span data-stu-id="c1e97-131">Request</span></span>
<span data-ttu-id="c1e97-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1e97-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="c1e97-133">响应</span><span class="sxs-lookup"><span data-stu-id="c1e97-133">Response</span></span>
<span data-ttu-id="c1e97-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1e97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






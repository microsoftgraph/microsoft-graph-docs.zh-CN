---
title: 列出 iosVppEBooks
description: 列出 iosVppEBook 对象的属性和关系。
ms.openlocfilehash: a0b69d40dcf5229a190d135cb5d154694d9d6771
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046608"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="dfc49-103">列出 iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="dfc49-103">List iosVppEBooks</span></span>

> <span data-ttu-id="dfc49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dfc49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfc49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dfc49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfc49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfc49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfc49-107">列出 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfc49-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfc49-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfc49-108">Prerequisites</span></span>
<span data-ttu-id="dfc49-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="dfc49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfc49-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfc49-111">Permission type</span></span>|<span data-ttu-id="dfc49-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfc49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfc49-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfc49-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc49-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dfc49-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfc49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc49-116">Not supported.</span></span>|
|<span data-ttu-id="dfc49-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfc49-117">Application</span></span>|<span data-ttu-id="dfc49-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfc49-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfc49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="dfc49-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfc49-120">Request headers</span></span>
|<span data-ttu-id="dfc49-121">标头</span><span class="sxs-lookup"><span data-stu-id="dfc49-121">Header</span></span>|<span data-ttu-id="dfc49-122">值</span><span class="sxs-lookup"><span data-stu-id="dfc49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfc49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfc49-123">Authorization</span></span>|<span data-ttu-id="dfc49-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfc49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfc49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dfc49-125">Accept</span></span>|<span data-ttu-id="dfc49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfc49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfc49-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfc49-127">Request body</span></span>
<span data-ttu-id="dfc49-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dfc49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc49-129">响应</span><span class="sxs-lookup"><span data-stu-id="dfc49-129">Response</span></span>
<span data-ttu-id="dfc49-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dfc49-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfc49-131">示例</span><span class="sxs-lookup"><span data-stu-id="dfc49-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfc49-132">请求</span><span class="sxs-lookup"><span data-stu-id="dfc49-132">Request</span></span>
<span data-ttu-id="dfc49-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfc49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="dfc49-134">响应</span><span class="sxs-lookup"><span data-stu-id="dfc49-134">Response</span></span>
<span data-ttu-id="dfc49-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfc49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1097

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
      "usedLicenseCount": 0
    }
  ]
}
```






---
title: 列出 managedMobileLobApps
description: 列出 managedMobileLobApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 32fbf9bb9d67726eec3f2853ef723887b759cd59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959620"
---
# <a name="list-managedmobilelobapps"></a><span data-ttu-id="61c61-103">列出 managedMobileLobApps</span><span class="sxs-lookup"><span data-stu-id="61c61-103">List managedMobileLobApps</span></span>

> <span data-ttu-id="61c61-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="61c61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61c61-105">列出 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61c61-105">List properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61c61-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="61c61-106">Prerequisites</span></span>
<span data-ttu-id="61c61-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="61c61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61c61-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="61c61-109">Permission type</span></span>|<span data-ttu-id="61c61-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="61c61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61c61-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61c61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61c61-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="61c61-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="61c61-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61c61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61c61-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="61c61-114">Not supported.</span></span>|
|<span data-ttu-id="61c61-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="61c61-115">Application</span></span>|<span data-ttu-id="61c61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="61c61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61c61-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61c61-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="61c61-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="61c61-118">Request headers</span></span>
|<span data-ttu-id="61c61-119">标头</span><span class="sxs-lookup"><span data-stu-id="61c61-119">Header</span></span>|<span data-ttu-id="61c61-120">值</span><span class="sxs-lookup"><span data-stu-id="61c61-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61c61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="61c61-121">Authorization</span></span>|<span data-ttu-id="61c61-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="61c61-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61c61-123">Accept</span><span class="sxs-lookup"><span data-stu-id="61c61-123">Accept</span></span>|<span data-ttu-id="61c61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="61c61-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61c61-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="61c61-125">Request body</span></span>
<span data-ttu-id="61c61-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61c61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61c61-127">响应</span><span class="sxs-lookup"><span data-stu-id="61c61-127">Response</span></span>
<span data-ttu-id="61c61-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="61c61-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61c61-129">示例</span><span class="sxs-lookup"><span data-stu-id="61c61-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="61c61-130">请求</span><span class="sxs-lookup"><span data-stu-id="61c61-130">Request</span></span>
<span data-ttu-id="61c61-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61c61-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="61c61-132">响应</span><span class="sxs-lookup"><span data-stu-id="61c61-132">Response</span></span>
<span data-ttu-id="61c61-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61c61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "value": [
    {
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
  ]
}
```




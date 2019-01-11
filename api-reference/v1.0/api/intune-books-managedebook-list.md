---
title: 列出 managedEBooks
description: 列出 managedEBook 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: baf4b7275d9c6709a2d8959d2f82b806d0df01f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807068"
---
# <a name="list-managedebooks"></a><span data-ttu-id="1ff37-103">列出 managedEBooks</span><span class="sxs-lookup"><span data-stu-id="1ff37-103">List managedEBooks</span></span>

> <span data-ttu-id="1ff37-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ff37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ff37-105">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ff37-105">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ff37-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ff37-106">Prerequisites</span></span>
<span data-ttu-id="1ff37-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1ff37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ff37-109">Permission type</span></span>|<span data-ttu-id="1ff37-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ff37-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff37-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff37-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1ff37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff37-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ff37-114">Not supported.</span></span>|
|<span data-ttu-id="1ff37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ff37-115">Application</span></span>|<span data-ttu-id="1ff37-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ff37-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ff37-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="1ff37-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ff37-118">Request headers</span></span>
|<span data-ttu-id="1ff37-119">标头</span><span class="sxs-lookup"><span data-stu-id="1ff37-119">Header</span></span>|<span data-ttu-id="1ff37-120">值</span><span class="sxs-lookup"><span data-stu-id="1ff37-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ff37-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ff37-121">Authorization</span></span>|<span data-ttu-id="1ff37-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ff37-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ff37-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1ff37-123">Accept</span></span>|<span data-ttu-id="1ff37-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff37-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff37-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ff37-125">Request body</span></span>
<span data-ttu-id="1ff37-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ff37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff37-127">响应</span><span class="sxs-lookup"><span data-stu-id="1ff37-127">Response</span></span>
<span data-ttu-id="1ff37-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedEBook](../resources/intune-books-managedebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ff37-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff37-129">示例</span><span class="sxs-lookup"><span data-stu-id="1ff37-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ff37-130">请求</span><span class="sxs-lookup"><span data-stu-id="1ff37-130">Request</span></span>
<span data-ttu-id="1ff37-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ff37-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="1ff37-132">响应</span><span class="sxs-lookup"><span data-stu-id="1ff37-132">Response</span></span>
<span data-ttu-id="1ff37-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ff37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```




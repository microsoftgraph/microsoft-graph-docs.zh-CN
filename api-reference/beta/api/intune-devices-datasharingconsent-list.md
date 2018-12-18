---
title: 列表 dataSharingConsents
description: 列出属性和 dataSharingConsent 对象之间的关系。
author: tfitzmac
ms.openlocfilehash: a8d3fd49b8749dc982b70601ae5fbff836d1052c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312619"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="0bd0a-103">列表 dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="0bd0a-103">List dataSharingConsents</span></span>

> <span data-ttu-id="0bd0a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bd0a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bd0a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bd0a-107">列出属性和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-107">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bd0a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0bd0a-108">Prerequisites</span></span>
<span data-ttu-id="0bd0a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0bd0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd0a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bd0a-111">Permission type</span></span>|<span data-ttu-id="0bd0a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0bd0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bd0a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bd0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bd0a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd0a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0bd0a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bd0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bd0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-116">Not supported.</span></span>|
|<span data-ttu-id="0bd0a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bd0a-117">Application</span></span>|<span data-ttu-id="0bd0a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bd0a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bd0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="0bd0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bd0a-120">Request headers</span></span>
|<span data-ttu-id="0bd0a-121">标头</span><span class="sxs-lookup"><span data-stu-id="0bd0a-121">Header</span></span>|<span data-ttu-id="0bd0a-122">值</span><span class="sxs-lookup"><span data-stu-id="0bd0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bd0a-123">授权</span><span class="sxs-lookup"><span data-stu-id="0bd0a-123">Authorization</span></span>|<span data-ttu-id="0bd0a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bd0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bd0a-125">Accept</span></span>|<span data-ttu-id="0bd0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bd0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bd0a-127">Request body</span></span>
<span data-ttu-id="0bd0a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bd0a-129">响应</span><span class="sxs-lookup"><span data-stu-id="0bd0a-129">Response</span></span>
<span data-ttu-id="0bd0a-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-130">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd0a-131">示例</span><span class="sxs-lookup"><span data-stu-id="0bd0a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bd0a-132">请求</span><span class="sxs-lookup"><span data-stu-id="0bd0a-132">Request</span></span>
<span data-ttu-id="0bd0a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="0bd0a-134">响应</span><span class="sxs-lookup"><span data-stu-id="0bd0a-134">Response</span></span>
<span data-ttu-id="0bd0a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bd0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "333387f7-87f7-3333-f787-3333f7873333",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```






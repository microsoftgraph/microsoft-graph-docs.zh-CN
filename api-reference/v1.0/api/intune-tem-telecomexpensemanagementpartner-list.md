---
title: 列出 telecomExpenseManagementPartners
description: 列出 telecomExpenseManagementPartner 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 5ef437d2aa8eb6a6f36f10e8951530fba1d5207d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349390"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="b8665-103">列出 telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="b8665-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="b8665-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8665-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8665-105">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8665-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8665-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8665-106">Prerequisites</span></span>
<span data-ttu-id="b8665-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b8665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8665-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8665-109">Permission type</span></span>|<span data-ttu-id="b8665-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8665-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8665-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8665-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8665-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8665-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b8665-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8665-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8665-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8665-114">Not supported.</span></span>|
|<span data-ttu-id="b8665-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8665-115">Application</span></span>|<span data-ttu-id="b8665-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8665-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8665-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8665-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="b8665-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8665-118">Request headers</span></span>
|<span data-ttu-id="b8665-119">标头</span><span class="sxs-lookup"><span data-stu-id="b8665-119">Header</span></span>|<span data-ttu-id="b8665-120">值</span><span class="sxs-lookup"><span data-stu-id="b8665-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8665-121">授权</span><span class="sxs-lookup"><span data-stu-id="b8665-121">Authorization</span></span>|<span data-ttu-id="b8665-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8665-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8665-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b8665-123">Accept</span></span>|<span data-ttu-id="b8665-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8665-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8665-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8665-125">Request body</span></span>
<span data-ttu-id="b8665-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8665-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8665-127">响应</span><span class="sxs-lookup"><span data-stu-id="b8665-127">Response</span></span>
<span data-ttu-id="b8665-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b8665-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8665-129">示例</span><span class="sxs-lookup"><span data-stu-id="b8665-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8665-130">请求</span><span class="sxs-lookup"><span data-stu-id="b8665-130">Request</span></span>
<span data-ttu-id="b8665-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8665-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="b8665-132">响应</span><span class="sxs-lookup"><span data-stu-id="b8665-132">Response</span></span>
<span data-ttu-id="b8665-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8665-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




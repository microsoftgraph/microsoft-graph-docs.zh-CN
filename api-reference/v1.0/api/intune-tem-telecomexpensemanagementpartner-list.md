---
title: 列出 telecomExpenseManagementPartners
description: 列出 telecomExpenseManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01b4089643e654f78063c71603cd8559239b1ae0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411015"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="24401-103">列出 telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="24401-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="24401-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24401-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24401-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24401-106">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24401-106">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24401-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="24401-107">Prerequisites</span></span>
<span data-ttu-id="24401-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24401-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="24401-110">Permission type</span></span>|<span data-ttu-id="24401-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24401-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24401-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24401-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24401-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24401-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="24401-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24401-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24401-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24401-115">Not supported.</span></span>|
|<span data-ttu-id="24401-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="24401-116">Application</span></span>|<span data-ttu-id="24401-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="24401-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24401-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24401-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="24401-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="24401-119">Request headers</span></span>
|<span data-ttu-id="24401-120">标头</span><span class="sxs-lookup"><span data-stu-id="24401-120">Header</span></span>|<span data-ttu-id="24401-121">值</span><span class="sxs-lookup"><span data-stu-id="24401-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24401-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24401-122">Authorization</span></span>|<span data-ttu-id="24401-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24401-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24401-124">接受</span><span class="sxs-lookup"><span data-stu-id="24401-124">Accept</span></span>|<span data-ttu-id="24401-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24401-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24401-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24401-126">Request body</span></span>
<span data-ttu-id="24401-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24401-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24401-128">响应</span><span class="sxs-lookup"><span data-stu-id="24401-128">Response</span></span>
<span data-ttu-id="24401-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="24401-129">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24401-130">示例</span><span class="sxs-lookup"><span data-stu-id="24401-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="24401-131">请求</span><span class="sxs-lookup"><span data-stu-id="24401-131">Request</span></span>
<span data-ttu-id="24401-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24401-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="24401-133">响应</span><span class="sxs-lookup"><span data-stu-id="24401-133">Response</span></span>
<span data-ttu-id="24401-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24401-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







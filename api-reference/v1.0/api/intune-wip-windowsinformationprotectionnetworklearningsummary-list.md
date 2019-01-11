---
title: 列出 windowsInformationProtectionNetworkLearningSummaries
description: 列出 windowsInformationProtectionNetworkLearningSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9b18e6c3a810fc2abe633ad1096ab9221cf379df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839191"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="46c7e-103">列出 windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="46c7e-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

> <span data-ttu-id="46c7e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="46c7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46c7e-105">列出 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="46c7e-105">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46c7e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="46c7e-106">Prerequisites</span></span>
<span data-ttu-id="46c7e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="46c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46c7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46c7e-109">Permission type</span></span>|<span data-ttu-id="46c7e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46c7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46c7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46c7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46c7e-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c7e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="46c7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46c7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46c7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c7e-114">Not supported.</span></span>|
|<span data-ttu-id="46c7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="46c7e-115">Application</span></span>|<span data-ttu-id="46c7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46c7e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46c7e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="46c7e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="46c7e-118">Request headers</span></span>
|<span data-ttu-id="46c7e-119">标头</span><span class="sxs-lookup"><span data-stu-id="46c7e-119">Header</span></span>|<span data-ttu-id="46c7e-120">值</span><span class="sxs-lookup"><span data-stu-id="46c7e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46c7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46c7e-121">Authorization</span></span>|<span data-ttu-id="46c7e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46c7e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46c7e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46c7e-123">Accept</span></span>|<span data-ttu-id="46c7e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46c7e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46c7e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="46c7e-125">Request body</span></span>
<span data-ttu-id="46c7e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46c7e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46c7e-127">响应</span><span class="sxs-lookup"><span data-stu-id="46c7e-127">Response</span></span>
<span data-ttu-id="46c7e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46c7e-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c7e-129">示例</span><span class="sxs-lookup"><span data-stu-id="46c7e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="46c7e-130">请求</span><span class="sxs-lookup"><span data-stu-id="46c7e-130">Request</span></span>
<span data-ttu-id="46c7e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46c7e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="46c7e-132">响应</span><span class="sxs-lookup"><span data-stu-id="46c7e-132">Response</span></span>
<span data-ttu-id="46c7e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
      "id": "242108f7-08f7-2421-f708-2124f7082124",
      "url": "Url value",
      "deviceCount": 11
    }
  ]
}
```




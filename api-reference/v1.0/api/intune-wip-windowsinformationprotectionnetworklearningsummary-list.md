---
title: 列出 windowsInformationProtectionNetworkLearningSummaries
description: 列出 windowsInformationProtectionNetworkLearningSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4b016a26510e571ba85c4d3c17bdf6b684333ce
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984791"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="c7f4a-103">列出 windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="c7f4a-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

> <span data-ttu-id="c7f4a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f4a-105">列出 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-105">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7f4a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7f4a-106">Prerequisites</span></span>
<span data-ttu-id="c7f4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f4a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7f4a-109">Permission type</span></span>|<span data-ttu-id="c7f4a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7f4a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7f4a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f4a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7f4a-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7f4a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c7f4a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f4a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7f4a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-114">Not supported.</span></span>|
|<span data-ttu-id="c7f4a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7f4a-115">Application</span></span>|<span data-ttu-id="c7f4a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7f4a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7f4a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c7f4a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7f4a-118">Request headers</span></span>
|<span data-ttu-id="c7f4a-119">标头</span><span class="sxs-lookup"><span data-stu-id="c7f4a-119">Header</span></span>|<span data-ttu-id="c7f4a-120">值</span><span class="sxs-lookup"><span data-stu-id="c7f4a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7f4a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7f4a-121">Authorization</span></span>|<span data-ttu-id="c7f4a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7f4a-123">接受</span><span class="sxs-lookup"><span data-stu-id="c7f4a-123">Accept</span></span>|<span data-ttu-id="c7f4a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7f4a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f4a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7f4a-125">Request body</span></span>
<span data-ttu-id="c7f4a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f4a-127">响应</span><span class="sxs-lookup"><span data-stu-id="c7f4a-127">Response</span></span>
<span data-ttu-id="c7f4a-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7f4a-129">示例</span><span class="sxs-lookup"><span data-stu-id="c7f4a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7f4a-130">请求</span><span class="sxs-lookup"><span data-stu-id="c7f4a-130">Request</span></span>
<span data-ttu-id="c7f4a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="c7f4a-132">响应</span><span class="sxs-lookup"><span data-stu-id="c7f4a-132">Response</span></span>
<span data-ttu-id="c7f4a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7f4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




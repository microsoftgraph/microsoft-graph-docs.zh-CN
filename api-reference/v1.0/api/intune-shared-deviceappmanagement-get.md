---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 269e749c7fae0b2eeb397d86907a7cf2d6653ee7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314194"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="6f0e1-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6f0e1-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="6f0e1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f0e1-105">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f0e1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f0e1-106">Prerequisites</span></span>

<span data-ttu-id="6f0e1-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6f0e1-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6f0e1-109">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6f0e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f0e1-110">Permission type</span></span>|<span data-ttu-id="6f0e1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f0e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f0e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f0e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f0e1-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f0e1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="6f0e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f0e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f0e1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-115">Not supported.</span></span>|
|<span data-ttu-id="6f0e1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f0e1-116">Application</span></span>|<span data-ttu-id="6f0e1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f0e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f0e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f0e1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f0e1-119">Optional query parameters</span></span>
<span data-ttu-id="6f0e1-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f0e1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f0e1-121">Request headers</span></span>
|<span data-ttu-id="6f0e1-122">标头</span><span class="sxs-lookup"><span data-stu-id="6f0e1-122">Header</span></span>|<span data-ttu-id="6f0e1-123">值</span><span class="sxs-lookup"><span data-stu-id="6f0e1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f0e1-124">授权</span><span class="sxs-lookup"><span data-stu-id="6f0e1-124">Authorization</span></span>|<span data-ttu-id="6f0e1-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f0e1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6f0e1-126">Accept</span></span>|<span data-ttu-id="6f0e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6f0e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f0e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f0e1-128">Request body</span></span>
<span data-ttu-id="6f0e1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f0e1-130">响应</span><span class="sxs-lookup"><span data-stu-id="6f0e1-130">Response</span></span>
<span data-ttu-id="6f0e1-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="6f0e1-132">示例请求</span><span class="sxs-lookup"><span data-stu-id="6f0e1-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="6f0e1-133">响应示例</span><span class="sxs-lookup"><span data-stu-id="6f0e1-133">Example response</span></span>
<span data-ttu-id="6f0e1-134">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6f0e1-135">从实际的呼叫，将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f0e1-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```




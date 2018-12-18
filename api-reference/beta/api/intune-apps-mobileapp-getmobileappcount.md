---
title: getMobileAppCount 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 35ff8211fee31938551cc8eb2fce72c79ce39bc9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358861"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="30910-103">getMobileAppCount 函数</span><span class="sxs-lookup"><span data-stu-id="30910-103">getMobileAppCount function</span></span>

> <span data-ttu-id="30910-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="30910-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30910-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="30910-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30910-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30910-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30910-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="30910-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30910-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="30910-108">Prerequisites</span></span>
<span data-ttu-id="30910-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="30910-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30910-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30910-111">Permission type</span></span>|<span data-ttu-id="30910-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30910-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30910-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30910-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30910-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30910-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="30910-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30910-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30910-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30910-116">Not supported.</span></span>|
|<span data-ttu-id="30910-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="30910-117">Application</span></span>|<span data-ttu-id="30910-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="30910-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30910-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30910-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="30910-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="30910-120">Request headers</span></span>
|<span data-ttu-id="30910-121">标头</span><span class="sxs-lookup"><span data-stu-id="30910-121">Header</span></span>|<span data-ttu-id="30910-122">值</span><span class="sxs-lookup"><span data-stu-id="30910-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30910-123">授权</span><span class="sxs-lookup"><span data-stu-id="30910-123">Authorization</span></span>|<span data-ttu-id="30910-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30910-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30910-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30910-125">Accept</span></span>|<span data-ttu-id="30910-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30910-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30910-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="30910-127">Request body</span></span>
<span data-ttu-id="30910-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="30910-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="30910-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="30910-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="30910-130">属性</span><span class="sxs-lookup"><span data-stu-id="30910-130">Property</span></span>|<span data-ttu-id="30910-131">类型</span><span class="sxs-lookup"><span data-stu-id="30910-131">Type</span></span>|<span data-ttu-id="30910-132">说明</span><span class="sxs-lookup"><span data-stu-id="30910-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30910-133">状态</span><span class="sxs-lookup"><span data-stu-id="30910-133">status</span></span>|<span data-ttu-id="30910-134">字符串</span><span class="sxs-lookup"><span data-stu-id="30910-134">String</span></span>|<span data-ttu-id="30910-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="30910-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="30910-136">响应</span><span class="sxs-lookup"><span data-stu-id="30910-136">Response</span></span>
<span data-ttu-id="30910-137">如果成功，此函数返回`200 OK`响应代码和响应正文中的 Int64。</span><span class="sxs-lookup"><span data-stu-id="30910-137">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30910-138">示例</span><span class="sxs-lookup"><span data-stu-id="30910-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="30910-139">请求</span><span class="sxs-lookup"><span data-stu-id="30910-139">Request</span></span>
<span data-ttu-id="30910-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30910-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="30910-141">响应</span><span class="sxs-lookup"><span data-stu-id="30910-141">Response</span></span>
<span data-ttu-id="30910-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30910-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```






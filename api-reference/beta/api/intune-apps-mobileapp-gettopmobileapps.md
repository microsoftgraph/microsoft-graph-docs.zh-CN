---
title: getTopMobileApps 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f5a380145c51ba61fe76638941c42352f254606e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980207"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="a915e-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="a915e-103">getTopMobileApps function</span></span>

> <span data-ttu-id="a915e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a915e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a915e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a915e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a915e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a915e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a915e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a915e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a915e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a915e-108">Prerequisites</span></span>
<span data-ttu-id="a915e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a915e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a915e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a915e-111">Permission type</span></span>|<span data-ttu-id="a915e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a915e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a915e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a915e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a915e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a915e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a915e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a915e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a915e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a915e-116">Not supported.</span></span>|
|<span data-ttu-id="a915e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a915e-117">Application</span></span>|<span data-ttu-id="a915e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a915e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a915e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a915e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a915e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a915e-120">Request headers</span></span>
|<span data-ttu-id="a915e-121">标头</span><span class="sxs-lookup"><span data-stu-id="a915e-121">Header</span></span>|<span data-ttu-id="a915e-122">值</span><span class="sxs-lookup"><span data-stu-id="a915e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a915e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a915e-123">Authorization</span></span>|<span data-ttu-id="a915e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a915e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a915e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a915e-125">Accept</span></span>|<span data-ttu-id="a915e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a915e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a915e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a915e-127">Request body</span></span>
<span data-ttu-id="a915e-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="a915e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a915e-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="a915e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a915e-130">属性</span><span class="sxs-lookup"><span data-stu-id="a915e-130">Property</span></span>|<span data-ttu-id="a915e-131">类型</span><span class="sxs-lookup"><span data-stu-id="a915e-131">Type</span></span>|<span data-ttu-id="a915e-132">说明</span><span class="sxs-lookup"><span data-stu-id="a915e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a915e-133">状态</span><span class="sxs-lookup"><span data-stu-id="a915e-133">status</span></span>|<span data-ttu-id="a915e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a915e-134">String</span></span>|<span data-ttu-id="a915e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a915e-135">Not yet documented</span></span>|
|<span data-ttu-id="a915e-136">count</span><span class="sxs-lookup"><span data-stu-id="a915e-136">count</span></span>|<span data-ttu-id="a915e-137">Int64</span><span class="sxs-lookup"><span data-stu-id="a915e-137">Int64</span></span>|<span data-ttu-id="a915e-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a915e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a915e-139">响应</span><span class="sxs-lookup"><span data-stu-id="a915e-139">Response</span></span>
<span data-ttu-id="a915e-140">如果成功，此函数返回`200 OK`响应代码和响应正文中的[mobileApp](../resources/intune-apps-mobileapp.md)集合。</span><span class="sxs-lookup"><span data-stu-id="a915e-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a915e-141">示例</span><span class="sxs-lookup"><span data-stu-id="a915e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a915e-142">请求</span><span class="sxs-lookup"><span data-stu-id="a915e-142">Request</span></span>
<span data-ttu-id="a915e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a915e-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="a915e-144">响应</span><span class="sxs-lookup"><span data-stu-id="a915e-144">Response</span></span>
<span data-ttu-id="a915e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a915e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "uploadState": 11,
      "publishingState": "processing"
    }
  ]
}
```






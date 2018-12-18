---
title: getTopMobileApps 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 03157e744358f4d76e781d33ae056104cf0a1130
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322727"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="bc44f-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="bc44f-103">getTopMobileApps function</span></span>

> <span data-ttu-id="bc44f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc44f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc44f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc44f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc44f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bc44f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc44f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc44f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc44f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc44f-108">Prerequisites</span></span>
<span data-ttu-id="bc44f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bc44f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc44f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc44f-111">Permission type</span></span>|<span data-ttu-id="bc44f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc44f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc44f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc44f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc44f-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc44f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bc44f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc44f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc44f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc44f-116">Not supported.</span></span>|
|<span data-ttu-id="bc44f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc44f-117">Application</span></span>|<span data-ttu-id="bc44f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc44f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc44f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc44f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bc44f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc44f-120">Request headers</span></span>
|<span data-ttu-id="bc44f-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc44f-121">Header</span></span>|<span data-ttu-id="bc44f-122">值</span><span class="sxs-lookup"><span data-stu-id="bc44f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc44f-123">授权</span><span class="sxs-lookup"><span data-stu-id="bc44f-123">Authorization</span></span>|<span data-ttu-id="bc44f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc44f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc44f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc44f-125">Accept</span></span>|<span data-ttu-id="bc44f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc44f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc44f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc44f-127">Request body</span></span>
<span data-ttu-id="bc44f-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="bc44f-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bc44f-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="bc44f-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bc44f-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc44f-130">Property</span></span>|<span data-ttu-id="bc44f-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc44f-131">Type</span></span>|<span data-ttu-id="bc44f-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc44f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc44f-133">状态</span><span class="sxs-lookup"><span data-stu-id="bc44f-133">status</span></span>|<span data-ttu-id="bc44f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bc44f-134">String</span></span>|<span data-ttu-id="bc44f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc44f-135">Not yet documented</span></span>|
|<span data-ttu-id="bc44f-136">count</span><span class="sxs-lookup"><span data-stu-id="bc44f-136">count</span></span>|<span data-ttu-id="bc44f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="bc44f-137">Int64</span></span>|<span data-ttu-id="bc44f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc44f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bc44f-139">响应</span><span class="sxs-lookup"><span data-stu-id="bc44f-139">Response</span></span>
<span data-ttu-id="bc44f-140">如果成功，此函数返回`200 OK`响应代码和响应正文中的[mobileApp](../resources/intune-apps-mobileapp.md)集合。</span><span class="sxs-lookup"><span data-stu-id="bc44f-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc44f-141">示例</span><span class="sxs-lookup"><span data-stu-id="bc44f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc44f-142">请求</span><span class="sxs-lookup"><span data-stu-id="bc44f-142">Request</span></span>
<span data-ttu-id="bc44f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc44f-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="bc44f-144">响应</span><span class="sxs-lookup"><span data-stu-id="bc44f-144">Response</span></span>
<span data-ttu-id="bc44f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc44f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






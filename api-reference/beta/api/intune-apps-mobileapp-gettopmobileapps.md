---
title: getTopMobileApps 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69874b6ccf94a78145c03279a5e6d13e0c45b995
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32490344"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="b69c3-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="b69c3-103">getTopMobileApps function</span></span>

> <span data-ttu-id="b69c3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b69c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b69c3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b69c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b69c3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b69c3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b69c3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b69c3-107">Prerequisites</span></span>
<span data-ttu-id="b69c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b69c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b69c3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b69c3-110">Permission type</span></span>|<span data-ttu-id="b69c3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b69c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b69c3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b69c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b69c3-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b69c3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b69c3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b69c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b69c3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b69c3-115">Not supported.</span></span>|
|<span data-ttu-id="b69c3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b69c3-116">Application</span></span>|<span data-ttu-id="b69c3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b69c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b69c3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b69c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b69c3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b69c3-119">Request headers</span></span>
|<span data-ttu-id="b69c3-120">标头</span><span class="sxs-lookup"><span data-stu-id="b69c3-120">Header</span></span>|<span data-ttu-id="b69c3-121">值</span><span class="sxs-lookup"><span data-stu-id="b69c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b69c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b69c3-122">Authorization</span></span>|<span data-ttu-id="b69c3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b69c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b69c3-124">接受</span><span class="sxs-lookup"><span data-stu-id="b69c3-124">Accept</span></span>|<span data-ttu-id="b69c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b69c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b69c3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b69c3-126">Request body</span></span>
<span data-ttu-id="b69c3-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b69c3-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b69c3-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b69c3-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b69c3-129">属性</span><span class="sxs-lookup"><span data-stu-id="b69c3-129">Property</span></span>|<span data-ttu-id="b69c3-130">类型</span><span class="sxs-lookup"><span data-stu-id="b69c3-130">Type</span></span>|<span data-ttu-id="b69c3-131">说明</span><span class="sxs-lookup"><span data-stu-id="b69c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b69c3-132">状态</span><span class="sxs-lookup"><span data-stu-id="b69c3-132">status</span></span>|<span data-ttu-id="b69c3-133">String</span><span class="sxs-lookup"><span data-stu-id="b69c3-133">String</span></span>|<span data-ttu-id="b69c3-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b69c3-134">Not yet documented</span></span>|
|<span data-ttu-id="b69c3-135">count</span><span class="sxs-lookup"><span data-stu-id="b69c3-135">count</span></span>|<span data-ttu-id="b69c3-136">Int64</span><span class="sxs-lookup"><span data-stu-id="b69c3-136">Int64</span></span>|<span data-ttu-id="b69c3-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b69c3-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b69c3-138">响应</span><span class="sxs-lookup"><span data-stu-id="b69c3-138">Response</span></span>
<span data-ttu-id="b69c3-139">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[mobileApp](../resources/intune-apps-mobileapp.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b69c3-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b69c3-140">示例</span><span class="sxs-lookup"><span data-stu-id="b69c3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b69c3-141">请求</span><span class="sxs-lookup"><span data-stu-id="b69c3-141">Request</span></span>
<span data-ttu-id="b69c3-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b69c3-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="b69c3-143">响应</span><span class="sxs-lookup"><span data-stu-id="b69c3-143">Response</span></span>
<span data-ttu-id="b69c3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b69c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

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
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1
    }
  ]
}
```






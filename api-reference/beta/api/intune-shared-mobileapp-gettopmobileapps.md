---
title: getTopMobileApps 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 426d79529414bd44f0a2327d503adf388943aaf5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865906"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="7a0db-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="7a0db-103">getTopMobileApps function</span></span>

<span data-ttu-id="7a0db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a0db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a0db-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a0db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a0db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a0db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a0db-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7a0db-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a0db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a0db-108">Prerequisites</span></span>
<span data-ttu-id="7a0db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a0db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a0db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a0db-111">Permission type</span></span>|<span data-ttu-id="7a0db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7a0db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a0db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a0db-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7a0db-114">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="7a0db-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7a0db-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a0db-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7a0db-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a0db-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a0db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a0db-117">Not supported.</span></span>|
|<span data-ttu-id="7a0db-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a0db-118">Application</span></span>||
| <span data-ttu-id="7a0db-119">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="7a0db-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7a0db-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a0db-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a0db-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a0db-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7a0db-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a0db-122">Request headers</span></span>
|<span data-ttu-id="7a0db-123">标头</span><span class="sxs-lookup"><span data-stu-id="7a0db-123">Header</span></span>|<span data-ttu-id="7a0db-124">值</span><span class="sxs-lookup"><span data-stu-id="7a0db-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a0db-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a0db-125">Authorization</span></span>|<span data-ttu-id="7a0db-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a0db-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a0db-127">接受</span><span class="sxs-lookup"><span data-stu-id="7a0db-127">Accept</span></span>|<span data-ttu-id="7a0db-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7a0db-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a0db-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a0db-129">Request body</span></span>
<span data-ttu-id="7a0db-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7a0db-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7a0db-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="7a0db-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7a0db-132">属性</span><span class="sxs-lookup"><span data-stu-id="7a0db-132">Property</span></span>|<span data-ttu-id="7a0db-133">类型</span><span class="sxs-lookup"><span data-stu-id="7a0db-133">Type</span></span>|<span data-ttu-id="7a0db-134">说明</span><span class="sxs-lookup"><span data-stu-id="7a0db-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a0db-135">状态</span><span class="sxs-lookup"><span data-stu-id="7a0db-135">status</span></span>|<span data-ttu-id="7a0db-136">String</span><span class="sxs-lookup"><span data-stu-id="7a0db-136">String</span></span>|<span data-ttu-id="7a0db-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7a0db-137">Not yet documented</span></span>|
|<span data-ttu-id="7a0db-138">count</span><span class="sxs-lookup"><span data-stu-id="7a0db-138">count</span></span>|<span data-ttu-id="7a0db-139">Int64</span><span class="sxs-lookup"><span data-stu-id="7a0db-139">Int64</span></span>|<span data-ttu-id="7a0db-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7a0db-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7a0db-141">响应</span><span class="sxs-lookup"><span data-stu-id="7a0db-141">Response</span></span>
<span data-ttu-id="7a0db-142">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [mobileApp](../resources/intune-shared-mobileapp.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="7a0db-142">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a0db-143">示例</span><span class="sxs-lookup"><span data-stu-id="7a0db-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a0db-144">请求</span><span class="sxs-lookup"><span data-stu-id="7a0db-144">Request</span></span>
<span data-ttu-id="7a0db-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a0db-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="7a0db-146">响应</span><span class="sxs-lookup"><span data-stu-id="7a0db-146">Response</span></span>
<span data-ttu-id="7a0db-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a0db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








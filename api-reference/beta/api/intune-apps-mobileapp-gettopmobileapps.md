---
title: getTopMobileApps 函数
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f29c6dfe6502b1520e2100781d47688bbbe5d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417026"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="5b5eb-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="5b5eb-103">getTopMobileApps function</span></span>

> <span data-ttu-id="5b5eb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b5eb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b5eb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b5eb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5b5eb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b5eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b5eb-108">Prerequisites</span></span>
<span data-ttu-id="5b5eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b5eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b5eb-111">Permission type</span></span>|<span data-ttu-id="5b5eb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b5eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b5eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b5eb-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b5eb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b5eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b5eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-116">Not supported.</span></span>|
|<span data-ttu-id="5b5eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b5eb-117">Application</span></span>|<span data-ttu-id="5b5eb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b5eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5b5eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b5eb-120">Request headers</span></span>
|<span data-ttu-id="5b5eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="5b5eb-121">Header</span></span>|<span data-ttu-id="5b5eb-122">值</span><span class="sxs-lookup"><span data-stu-id="5b5eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b5eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b5eb-123">Authorization</span></span>|<span data-ttu-id="5b5eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b5eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b5eb-125">Accept</span></span>|<span data-ttu-id="5b5eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b5eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b5eb-127">Request body</span></span>
<span data-ttu-id="5b5eb-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5b5eb-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5b5eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="5b5eb-130">Property</span></span>|<span data-ttu-id="5b5eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="5b5eb-131">Type</span></span>|<span data-ttu-id="5b5eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="5b5eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5eb-133">状态</span><span class="sxs-lookup"><span data-stu-id="5b5eb-133">status</span></span>|<span data-ttu-id="5b5eb-134">String</span><span class="sxs-lookup"><span data-stu-id="5b5eb-134">String</span></span>|<span data-ttu-id="5b5eb-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5b5eb-135">Not yet documented</span></span>|
|<span data-ttu-id="5b5eb-136">count</span><span class="sxs-lookup"><span data-stu-id="5b5eb-136">count</span></span>|<span data-ttu-id="5b5eb-137">Int64</span><span class="sxs-lookup"><span data-stu-id="5b5eb-137">Int64</span></span>|<span data-ttu-id="5b5eb-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5b5eb-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5b5eb-139">响应</span><span class="sxs-lookup"><span data-stu-id="5b5eb-139">Response</span></span>
<span data-ttu-id="5b5eb-140">如果成功，此函数返回`200 OK`响应代码和响应正文中的[mobileApp](../resources/intune-apps-mobileapp.md)集合。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b5eb-141">示例</span><span class="sxs-lookup"><span data-stu-id="5b5eb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b5eb-142">请求</span><span class="sxs-lookup"><span data-stu-id="5b5eb-142">Request</span></span>
<span data-ttu-id="5b5eb-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="5b5eb-144">响应</span><span class="sxs-lookup"><span data-stu-id="5b5eb-144">Response</span></span>
<span data-ttu-id="5b5eb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b5eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

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
      ]
    }
  ]
}
```





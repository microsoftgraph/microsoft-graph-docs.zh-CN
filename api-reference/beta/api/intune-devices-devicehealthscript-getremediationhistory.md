---
title: getRemediationHistory 函数
description: 用于获取设备运行状况脚本的 remediations 数的函数
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5469f8c5c4ae35d69e92b6d1e007bf4a0b3703ea
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176979"
---
# <a name="getremediationhistory-function"></a><span data-ttu-id="602af-103">getRemediationHistory 函数</span><span class="sxs-lookup"><span data-stu-id="602af-103">getRemediationHistory function</span></span>

<span data-ttu-id="602af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="602af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="602af-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="602af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="602af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="602af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="602af-107">用于获取设备运行状况脚本的 remediations 数的函数</span><span class="sxs-lookup"><span data-stu-id="602af-107">Function to get the number of remediations by a device health scripts</span></span>

## <a name="prerequisites"></a><span data-ttu-id="602af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="602af-108">Prerequisites</span></span>
<span data-ttu-id="602af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="602af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="602af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="602af-111">Permission type</span></span>|<span data-ttu-id="602af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="602af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="602af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="602af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="602af-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="602af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="602af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="602af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="602af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="602af-116">Not supported.</span></span>|
|<span data-ttu-id="602af-117">Application</span><span class="sxs-lookup"><span data-stu-id="602af-117">Application</span></span>|<span data-ttu-id="602af-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="602af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="602af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="602af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

## <a name="request-headers"></a><span data-ttu-id="602af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="602af-120">Request headers</span></span>
|<span data-ttu-id="602af-121">标头</span><span class="sxs-lookup"><span data-stu-id="602af-121">Header</span></span>|<span data-ttu-id="602af-122">值</span><span class="sxs-lookup"><span data-stu-id="602af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="602af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="602af-123">Authorization</span></span>|<span data-ttu-id="602af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="602af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="602af-125">接受</span><span class="sxs-lookup"><span data-stu-id="602af-125">Accept</span></span>|<span data-ttu-id="602af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="602af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="602af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="602af-127">Request body</span></span>
<span data-ttu-id="602af-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="602af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="602af-129">响应</span><span class="sxs-lookup"><span data-stu-id="602af-129">Response</span></span>
<span data-ttu-id="602af-130">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) 。</span><span class="sxs-lookup"><span data-stu-id="602af-130">If successful, this function returns a `200 OK` response code and a [deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="602af-131">示例</span><span class="sxs-lookup"><span data-stu-id="602af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="602af-132">请求</span><span class="sxs-lookup"><span data-stu-id="602af-132">Request</span></span>
<span data-ttu-id="602af-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="602af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

### <a name="response"></a><span data-ttu-id="602af-134">响应</span><span class="sxs-lookup"><span data-stu-id="602af-134">Response</span></span>
<span data-ttu-id="602af-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="602af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "historyData": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
        "date": "2016-12-31",
        "remediatedDeviceCount": 5,
        "noIssueDeviceCount": 2
      }
    ]
  }
}
```




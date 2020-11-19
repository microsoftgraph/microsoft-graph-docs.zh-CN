---
title: 获取 deviceHealthScriptRunSummary
description: 读取 deviceHealthScriptRunSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d61e62fa513e7d8921ffa71e5690089be3d8577
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235075"
---
# <a name="get-devicehealthscriptrunsummary"></a><span data-ttu-id="6cfa7-103">获取 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="6cfa7-103">Get deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="6cfa7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cfa7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cfa7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cfa7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cfa7-107">读取 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-107">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cfa7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6cfa7-108">Prerequisites</span></span>
<span data-ttu-id="6cfa7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cfa7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cfa7-111">Permission type</span></span>|<span data-ttu-id="6cfa7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6cfa7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cfa7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cfa7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cfa7-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfa7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cfa7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cfa7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cfa7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-116">Not supported.</span></span>|
|<span data-ttu-id="6cfa7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cfa7-117">Application</span></span>|<span data-ttu-id="6cfa7-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cfa7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cfa7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cfa7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cfa7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6cfa7-120">Optional query parameters</span></span>
<span data-ttu-id="6cfa7-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cfa7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cfa7-122">Request headers</span></span>
|<span data-ttu-id="6cfa7-123">标头</span><span class="sxs-lookup"><span data-stu-id="6cfa7-123">Header</span></span>|<span data-ttu-id="6cfa7-124">值</span><span class="sxs-lookup"><span data-stu-id="6cfa7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cfa7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cfa7-125">Authorization</span></span>|<span data-ttu-id="6cfa7-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cfa7-127">接受</span><span class="sxs-lookup"><span data-stu-id="6cfa7-127">Accept</span></span>|<span data-ttu-id="6cfa7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6cfa7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cfa7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cfa7-129">Request body</span></span>
<span data-ttu-id="6cfa7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cfa7-131">响应</span><span class="sxs-lookup"><span data-stu-id="6cfa7-131">Response</span></span>
<span data-ttu-id="6cfa7-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cfa7-133">示例</span><span class="sxs-lookup"><span data-stu-id="6cfa7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cfa7-134">请求</span><span class="sxs-lookup"><span data-stu-id="6cfa7-134">Request</span></span>
<span data-ttu-id="6cfa7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="6cfa7-136">响应</span><span class="sxs-lookup"><span data-stu-id="6cfa7-136">Response</span></span>
<span data-ttu-id="6cfa7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6cfa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 586

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
    "id": "8221b043-b043-8221-43b0-218243b02182",
    "noIssueDetectedDeviceCount": 10,
    "issueDetectedDeviceCount": 8,
    "detectionScriptErrorDeviceCount": 15,
    "detectionScriptPendingDeviceCount": 1,
    "issueRemediatedDeviceCount": 10,
    "remediationSkippedDeviceCount": 13,
    "issueReoccurredDeviceCount": 10,
    "remediationScriptErrorDeviceCount": 1,
    "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
    "issueRemediatedCumulativeDeviceCount": 4
  }
}
```





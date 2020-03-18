---
title: 获取 deviceManagementScriptRunSummary
description: 读取 deviceManagementScriptRunSummary 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8374bae4cc9675ce526dfdf4c559c4b075d487d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814391"
---
# <a name="get-devicemanagementscriptrunsummary"></a><span data-ttu-id="ecc3b-103">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="ecc3b-103">Get deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="ecc3b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecc3b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecc3b-106">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-106">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecc3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecc3b-107">Prerequisites</span></span>
<span data-ttu-id="ecc3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecc3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecc3b-110">Permission type</span></span>|<span data-ttu-id="ecc3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecc3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecc3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecc3b-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecc3b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ecc3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecc3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-115">Not supported.</span></span>|
|<span data-ttu-id="ecc3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecc3b-116">Application</span></span>|<span data-ttu-id="ecc3b-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecc3b-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecc3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecc3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecc3b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ecc3b-119">Optional query parameters</span></span>
<span data-ttu-id="ecc3b-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecc3b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecc3b-121">Request headers</span></span>
|<span data-ttu-id="ecc3b-122">标头</span><span class="sxs-lookup"><span data-stu-id="ecc3b-122">Header</span></span>|<span data-ttu-id="ecc3b-123">值</span><span class="sxs-lookup"><span data-stu-id="ecc3b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecc3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecc3b-124">Authorization</span></span>|<span data-ttu-id="ecc3b-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecc3b-126">接受</span><span class="sxs-lookup"><span data-stu-id="ecc3b-126">Accept</span></span>|<span data-ttu-id="ecc3b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ecc3b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecc3b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecc3b-128">Request body</span></span>
<span data-ttu-id="ecc3b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc3b-130">响应</span><span class="sxs-lookup"><span data-stu-id="ecc3b-130">Response</span></span>
<span data-ttu-id="ecc3b-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecc3b-132">示例</span><span class="sxs-lookup"><span data-stu-id="ecc3b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecc3b-133">请求</span><span class="sxs-lookup"><span data-stu-id="ecc3b-133">Request</span></span>
<span data-ttu-id="ecc3b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="ecc3b-135">响应</span><span class="sxs-lookup"><span data-stu-id="ecc3b-135">Response</span></span>
<span data-ttu-id="ecc3b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecc3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
    "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "successUserCount": 0,
    "errorUserCount": 14
  }
}
```





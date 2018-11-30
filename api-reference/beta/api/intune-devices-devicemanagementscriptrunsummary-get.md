---
title: 获取 deviceManagementScriptRunSummary
description: 读取属性和 deviceManagementScriptRunSummary 对象的关系。
ms.openlocfilehash: ab9f62aefce2c71e2776c6dfca5f50105a2fbc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044597"
---
# <a name="get-devicemanagementscriptrunsummary"></a><span data-ttu-id="c5514-103">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c5514-103">Get deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="c5514-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5514-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5514-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5514-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5514-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c5514-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5514-107">读取属性和[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c5514-107">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5514-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5514-108">Prerequisites</span></span>
<span data-ttu-id="c5514-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c5514-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5514-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5514-111">Permission type</span></span>|<span data-ttu-id="c5514-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5514-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5514-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5514-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5514-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5514-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c5514-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5514-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5514-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5514-116">Not supported.</span></span>|
|<span data-ttu-id="c5514-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5514-117">Application</span></span>|<span data-ttu-id="c5514-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5514-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5514-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5514-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5514-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5514-120">Optional query parameters</span></span>
<span data-ttu-id="c5514-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5514-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c5514-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5514-122">Request headers</span></span>
|<span data-ttu-id="c5514-123">标头</span><span class="sxs-lookup"><span data-stu-id="c5514-123">Header</span></span>|<span data-ttu-id="c5514-124">值</span><span class="sxs-lookup"><span data-stu-id="c5514-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5514-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5514-125">Authorization</span></span>|<span data-ttu-id="c5514-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5514-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5514-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c5514-127">Accept</span></span>|<span data-ttu-id="c5514-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5514-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5514-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5514-129">Request body</span></span>
<span data-ttu-id="c5514-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5514-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5514-131">响应</span><span class="sxs-lookup"><span data-stu-id="c5514-131">Response</span></span>
<span data-ttu-id="c5514-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5514-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5514-133">示例</span><span class="sxs-lookup"><span data-stu-id="c5514-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5514-134">请求</span><span class="sxs-lookup"><span data-stu-id="c5514-134">Request</span></span>
<span data-ttu-id="c5514-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5514-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="c5514-136">响应</span><span class="sxs-lookup"><span data-stu-id="c5514-136">Response</span></span>
<span data-ttu-id="c5514-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5514-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






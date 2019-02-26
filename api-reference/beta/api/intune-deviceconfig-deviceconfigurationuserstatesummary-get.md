---
title: 获取 deviceConfigurationUserStateSummary
description: 读取 deviceConfigurationUserStateSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14bab0f13da6a7d2ac6d906e396591b36dc4625c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162620"
---
# <a name="get-deviceconfigurationuserstatesummary"></a><span data-ttu-id="86495-103">获取 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="86495-103">Get deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="86495-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86495-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86495-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86495-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86495-106">读取[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86495-106">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86495-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86495-107">Prerequisites</span></span>
<span data-ttu-id="86495-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="86495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86495-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86495-110">Permission type</span></span>|<span data-ttu-id="86495-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86495-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86495-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86495-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86495-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86495-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="86495-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86495-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86495-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86495-115">Not supported.</span></span>|
|<span data-ttu-id="86495-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86495-116">Application</span></span>|<span data-ttu-id="86495-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="86495-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86495-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86495-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86495-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86495-119">Optional query parameters</span></span>
<span data-ttu-id="86495-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86495-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86495-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="86495-121">Request headers</span></span>
|<span data-ttu-id="86495-122">标头</span><span class="sxs-lookup"><span data-stu-id="86495-122">Header</span></span>|<span data-ttu-id="86495-123">值</span><span class="sxs-lookup"><span data-stu-id="86495-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86495-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="86495-124">Authorization</span></span>|<span data-ttu-id="86495-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86495-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86495-126">Accept</span><span class="sxs-lookup"><span data-stu-id="86495-126">Accept</span></span>|<span data-ttu-id="86495-127">application/json</span><span class="sxs-lookup"><span data-stu-id="86495-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86495-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="86495-128">Request body</span></span>
<span data-ttu-id="86495-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86495-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86495-130">响应</span><span class="sxs-lookup"><span data-stu-id="86495-130">Response</span></span>
<span data-ttu-id="86495-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86495-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86495-132">示例</span><span class="sxs-lookup"><span data-stu-id="86495-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="86495-133">请求</span><span class="sxs-lookup"><span data-stu-id="86495-133">Request</span></span>
<span data-ttu-id="86495-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86495-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
```

### <a name="response"></a><span data-ttu-id="86495-135">响应</span><span class="sxs-lookup"><span data-stu-id="86495-135">Response</span></span>
<span data-ttu-id="86495-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86495-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 361

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
    "id": "e8957887-7887-e895-8778-95e8877895e8",
    "unknownUserCount": 0,
    "notApplicableUserCount": 6,
    "compliantUserCount": 2,
    "remediatedUserCount": 3,
    "nonCompliantUserCount": 5,
    "errorUserCount": 14,
    "conflictUserCount": 1
  }
}
```





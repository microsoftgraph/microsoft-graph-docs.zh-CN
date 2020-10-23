---
title: 获取 deviceConfigurationUserStateSummary
description: 读取 deviceConfigurationUserStateSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05fc6649b10ac849c120c927f511392929f3ba93
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730013"
---
# <a name="get-deviceconfigurationuserstatesummary"></a><span data-ttu-id="b45e5-103">获取 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="b45e5-103">Get deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="b45e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b45e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b45e5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b45e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b45e5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b45e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b45e5-107">读取 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b45e5-107">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b45e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b45e5-108">Prerequisites</span></span>
<span data-ttu-id="b45e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b45e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b45e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b45e5-111">Permission type</span></span>|<span data-ttu-id="b45e5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b45e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b45e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b45e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b45e5-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b45e5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b45e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b45e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b45e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b45e5-116">Not supported.</span></span>|
|<span data-ttu-id="b45e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b45e5-117">Application</span></span>|<span data-ttu-id="b45e5-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b45e5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b45e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b45e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b45e5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b45e5-120">Optional query parameters</span></span>
<span data-ttu-id="b45e5-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b45e5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b45e5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b45e5-122">Request headers</span></span>
|<span data-ttu-id="b45e5-123">标头</span><span class="sxs-lookup"><span data-stu-id="b45e5-123">Header</span></span>|<span data-ttu-id="b45e5-124">值</span><span class="sxs-lookup"><span data-stu-id="b45e5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b45e5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b45e5-125">Authorization</span></span>|<span data-ttu-id="b45e5-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b45e5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b45e5-127">接受</span><span class="sxs-lookup"><span data-stu-id="b45e5-127">Accept</span></span>|<span data-ttu-id="b45e5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b45e5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45e5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b45e5-129">Request body</span></span>
<span data-ttu-id="b45e5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b45e5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b45e5-131">响应</span><span class="sxs-lookup"><span data-stu-id="b45e5-131">Response</span></span>
<span data-ttu-id="b45e5-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b45e5-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b45e5-133">示例</span><span class="sxs-lookup"><span data-stu-id="b45e5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b45e5-134">请求</span><span class="sxs-lookup"><span data-stu-id="b45e5-134">Request</span></span>
<span data-ttu-id="b45e5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b45e5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
```

### <a name="response"></a><span data-ttu-id="b45e5-136">响应</span><span class="sxs-lookup"><span data-stu-id="b45e5-136">Response</span></span>
<span data-ttu-id="b45e5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b45e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






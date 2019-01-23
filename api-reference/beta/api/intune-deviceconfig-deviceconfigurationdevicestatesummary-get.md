---
title: 获取 deviceConfigurationDeviceStateSummary
description: 读取 deviceConfigurationDeviceStateSummary 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17fd2e19b9a23d20ecbd5c4cb44c01add264009
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401255"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="1d188-103">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1d188-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="1d188-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1d188-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d188-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d188-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d188-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d188-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d188-107">读取 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d188-107">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d188-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d188-108">Prerequisites</span></span>
<span data-ttu-id="1d188-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1d188-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d188-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d188-111">Permission type</span></span>|<span data-ttu-id="1d188-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d188-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d188-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d188-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d188-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d188-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1d188-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d188-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d188-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d188-116">Not supported.</span></span>|
|<span data-ttu-id="1d188-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d188-117">Application</span></span>|<span data-ttu-id="1d188-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d188-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d188-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d188-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d188-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d188-120">Optional query parameters</span></span>
<span data-ttu-id="1d188-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d188-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d188-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d188-122">Request headers</span></span>
|<span data-ttu-id="1d188-123">标头</span><span class="sxs-lookup"><span data-stu-id="1d188-123">Header</span></span>|<span data-ttu-id="1d188-124">值</span><span class="sxs-lookup"><span data-stu-id="1d188-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d188-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d188-125">Authorization</span></span>|<span data-ttu-id="1d188-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d188-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d188-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1d188-127">Accept</span></span>|<span data-ttu-id="1d188-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d188-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d188-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d188-129">Request body</span></span>
<span data-ttu-id="1d188-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d188-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d188-131">响应</span><span class="sxs-lookup"><span data-stu-id="1d188-131">Response</span></span>
<span data-ttu-id="1d188-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d188-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d188-133">示例</span><span class="sxs-lookup"><span data-stu-id="1d188-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d188-134">请求</span><span class="sxs-lookup"><span data-stu-id="1d188-134">Request</span></span>
<span data-ttu-id="1d188-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d188-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="1d188-136">响应</span><span class="sxs-lookup"><span data-stu-id="1d188-136">Response</span></span>
<span data-ttu-id="1d188-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d188-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```





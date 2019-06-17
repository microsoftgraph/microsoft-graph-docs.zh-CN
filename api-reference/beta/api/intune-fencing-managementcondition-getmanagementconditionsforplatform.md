---
title: getManagementConditionsForPlatform 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ade52245e67ce6628a9ff0cdf580523247f8e671
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984112"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="b490f-103">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="b490f-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="b490f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b490f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b490f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b490f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b490f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b490f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b490f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b490f-107">Prerequisites</span></span>
<span data-ttu-id="b490f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b490f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b490f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b490f-110">Permission type</span></span>|<span data-ttu-id="b490f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b490f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b490f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b490f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b490f-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b490f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b490f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b490f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b490f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b490f-115">Not supported.</span></span>|
|<span data-ttu-id="b490f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b490f-116">Application</span></span>|<span data-ttu-id="b490f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b490f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b490f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b490f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="b490f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b490f-119">Request headers</span></span>
|<span data-ttu-id="b490f-120">标头</span><span class="sxs-lookup"><span data-stu-id="b490f-120">Header</span></span>|<span data-ttu-id="b490f-121">值</span><span class="sxs-lookup"><span data-stu-id="b490f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b490f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b490f-122">Authorization</span></span>|<span data-ttu-id="b490f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b490f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b490f-124">接受</span><span class="sxs-lookup"><span data-stu-id="b490f-124">Accept</span></span>|<span data-ttu-id="b490f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b490f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b490f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b490f-126">Request body</span></span>
<span data-ttu-id="b490f-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b490f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b490f-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b490f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b490f-129">属性</span><span class="sxs-lookup"><span data-stu-id="b490f-129">Property</span></span>|<span data-ttu-id="b490f-130">类型</span><span class="sxs-lookup"><span data-stu-id="b490f-130">Type</span></span>|<span data-ttu-id="b490f-131">说明</span><span class="sxs-lookup"><span data-stu-id="b490f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b490f-132">platform</span><span class="sxs-lookup"><span data-stu-id="b490f-132">platform</span></span>|[<span data-ttu-id="b490f-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="b490f-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="b490f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b490f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b490f-135">响应</span><span class="sxs-lookup"><span data-stu-id="b490f-135">Response</span></span>
<span data-ttu-id="b490f-136">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[managementCondition](../resources/intune-fencing-managementcondition.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b490f-136">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b490f-137">示例</span><span class="sxs-lookup"><span data-stu-id="b490f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b490f-138">请求</span><span class="sxs-lookup"><span data-stu-id="b490f-138">Request</span></span>
<span data-ttu-id="b490f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b490f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b490f-140">响应</span><span class="sxs-lookup"><span data-stu-id="b490f-140">Response</span></span>
<span data-ttu-id="b490f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b490f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```






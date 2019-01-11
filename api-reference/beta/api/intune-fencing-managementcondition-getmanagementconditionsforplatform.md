---
title: getManagementConditionsForPlatform 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13871db2f5dd99de80caf1004baa96aaf6dcf146
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864923"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="89a87-103">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="89a87-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="89a87-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89a87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89a87-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89a87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89a87-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89a87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89a87-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89a87-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89a87-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89a87-108">Prerequisites</span></span>
<span data-ttu-id="89a87-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="89a87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89a87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89a87-111">Permission type</span></span>|<span data-ttu-id="89a87-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89a87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89a87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89a87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89a87-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89a87-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89a87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89a87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89a87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a87-116">Not supported.</span></span>|
|<span data-ttu-id="89a87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89a87-117">Application</span></span>|<span data-ttu-id="89a87-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89a87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89a87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="89a87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89a87-120">Request headers</span></span>
|<span data-ttu-id="89a87-121">标头</span><span class="sxs-lookup"><span data-stu-id="89a87-121">Header</span></span>|<span data-ttu-id="89a87-122">值</span><span class="sxs-lookup"><span data-stu-id="89a87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89a87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89a87-123">Authorization</span></span>|<span data-ttu-id="89a87-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89a87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89a87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89a87-125">Accept</span></span>|<span data-ttu-id="89a87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89a87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89a87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89a87-127">Request body</span></span>
<span data-ttu-id="89a87-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="89a87-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="89a87-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="89a87-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="89a87-130">属性</span><span class="sxs-lookup"><span data-stu-id="89a87-130">Property</span></span>|<span data-ttu-id="89a87-131">类型</span><span class="sxs-lookup"><span data-stu-id="89a87-131">Type</span></span>|<span data-ttu-id="89a87-132">Description</span><span class="sxs-lookup"><span data-stu-id="89a87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a87-133">platform</span><span class="sxs-lookup"><span data-stu-id="89a87-133">platform</span></span>|[<span data-ttu-id="89a87-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="89a87-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="89a87-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89a87-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89a87-136">响应</span><span class="sxs-lookup"><span data-stu-id="89a87-136">Response</span></span>
<span data-ttu-id="89a87-137">如果成功，此函数返回`200 OK`响应代码和响应正文中的[managementCondition](../resources/intune-fencing-managementcondition.md)集合。</span><span class="sxs-lookup"><span data-stu-id="89a87-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89a87-138">示例</span><span class="sxs-lookup"><span data-stu-id="89a87-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="89a87-139">请求</span><span class="sxs-lookup"><span data-stu-id="89a87-139">Request</span></span>
<span data-ttu-id="89a87-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89a87-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="89a87-141">响应</span><span class="sxs-lookup"><span data-stu-id="89a87-141">Response</span></span>
<span data-ttu-id="89a87-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89a87-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






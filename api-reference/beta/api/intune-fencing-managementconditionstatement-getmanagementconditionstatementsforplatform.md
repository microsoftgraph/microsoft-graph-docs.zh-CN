---
title: getManagementConditionStatementsForPlatform 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c45382e5d2f7155be45c07c3846cd15fdec9b56f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054110"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="cca98-103">getManagementConditionStatementsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="cca98-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="cca98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cca98-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cca98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cca98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cca98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cca98-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cca98-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cca98-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cca98-108">Prerequisites</span></span>
<span data-ttu-id="cca98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cca98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cca98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cca98-111">Permission type</span></span>|<span data-ttu-id="cca98-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cca98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cca98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cca98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cca98-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca98-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cca98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cca98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cca98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cca98-116">Not supported.</span></span>|
|<span data-ttu-id="cca98-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cca98-117">Application</span></span>|<span data-ttu-id="cca98-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca98-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cca98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cca98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="cca98-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cca98-120">Request headers</span></span>
|<span data-ttu-id="cca98-121">标头</span><span class="sxs-lookup"><span data-stu-id="cca98-121">Header</span></span>|<span data-ttu-id="cca98-122">值</span><span class="sxs-lookup"><span data-stu-id="cca98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cca98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cca98-123">Authorization</span></span>|<span data-ttu-id="cca98-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cca98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cca98-125">接受</span><span class="sxs-lookup"><span data-stu-id="cca98-125">Accept</span></span>|<span data-ttu-id="cca98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cca98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cca98-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cca98-127">Request body</span></span>
<span data-ttu-id="cca98-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="cca98-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cca98-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="cca98-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cca98-130">属性</span><span class="sxs-lookup"><span data-stu-id="cca98-130">Property</span></span>|<span data-ttu-id="cca98-131">类型</span><span class="sxs-lookup"><span data-stu-id="cca98-131">Type</span></span>|<span data-ttu-id="cca98-132">说明</span><span class="sxs-lookup"><span data-stu-id="cca98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cca98-133">平台</span><span class="sxs-lookup"><span data-stu-id="cca98-133">platform</span></span>|[<span data-ttu-id="cca98-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="cca98-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="cca98-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cca98-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cca98-136">响应</span><span class="sxs-lookup"><span data-stu-id="cca98-136">Response</span></span>
<span data-ttu-id="cca98-137">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="cca98-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca98-138">示例</span><span class="sxs-lookup"><span data-stu-id="cca98-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cca98-139">请求</span><span class="sxs-lookup"><span data-stu-id="cca98-139">Request</span></span>
<span data-ttu-id="cca98-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cca98-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cca98-141">响应</span><span class="sxs-lookup"><span data-stu-id="cca98-141">Response</span></span>
<span data-ttu-id="cca98-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cca98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpressionString",
        "value": "Value value"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```







---
title: getManagementConditionsForPlatform 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0b7d2f1ffdbe7dba4fbde09d80883fa60b5abaa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153732"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="d6bde-103">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="d6bde-103">getManagementConditionsForPlatform function</span></span>

<span data-ttu-id="d6bde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6bde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6bde-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6bde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bde-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6bde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bde-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d6bde-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6bde-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6bde-108">Prerequisites</span></span>
<span data-ttu-id="d6bde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6bde-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6bde-111">Permission type</span></span>|<span data-ttu-id="d6bde-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6bde-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6bde-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6bde-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bde-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6bde-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6bde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6bde-116">Not supported.</span></span>|
|<span data-ttu-id="d6bde-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6bde-117">Application</span></span>|<span data-ttu-id="d6bde-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bde-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6bde-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6bde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="d6bde-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6bde-120">Request headers</span></span>
|<span data-ttu-id="d6bde-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6bde-121">Header</span></span>|<span data-ttu-id="d6bde-122">值</span><span class="sxs-lookup"><span data-stu-id="d6bde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6bde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6bde-123">Authorization</span></span>|<span data-ttu-id="d6bde-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6bde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6bde-125">接受</span><span class="sxs-lookup"><span data-stu-id="d6bde-125">Accept</span></span>|<span data-ttu-id="d6bde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6bde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6bde-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6bde-127">Request body</span></span>
<span data-ttu-id="d6bde-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d6bde-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d6bde-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d6bde-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d6bde-130">属性</span><span class="sxs-lookup"><span data-stu-id="d6bde-130">Property</span></span>|<span data-ttu-id="d6bde-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6bde-131">Type</span></span>|<span data-ttu-id="d6bde-132">说明</span><span class="sxs-lookup"><span data-stu-id="d6bde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bde-133">平台</span><span class="sxs-lookup"><span data-stu-id="d6bde-133">platform</span></span>|[<span data-ttu-id="d6bde-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d6bde-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d6bde-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d6bde-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6bde-136">响应</span><span class="sxs-lookup"><span data-stu-id="d6bde-136">Response</span></span>
<span data-ttu-id="d6bde-137">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [managementCondition](../resources/intune-fencing-managementcondition.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d6bde-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6bde-138">示例</span><span class="sxs-lookup"><span data-stu-id="d6bde-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6bde-139">请求</span><span class="sxs-lookup"><span data-stu-id="d6bde-139">Request</span></span>
<span data-ttu-id="d6bde-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6bde-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d6bde-141">响应</span><span class="sxs-lookup"><span data-stu-id="d6bde-141">Response</span></span>
<span data-ttu-id="d6bde-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6bde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





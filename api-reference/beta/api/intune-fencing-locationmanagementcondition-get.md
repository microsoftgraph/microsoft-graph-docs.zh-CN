---
title: 获取 locationManagementCondition
description: 读取属性和 locationManagementCondition 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1bf6476fb1dad5db06f239df5594205f859b34df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841235"
---
# <a name="get-locationmanagementcondition"></a><span data-ttu-id="1f6ef-103">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1f6ef-103">Get locationManagementCondition</span></span>

> <span data-ttu-id="1f6ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f6ef-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f6ef-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f6ef-107">读取属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-107">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f6ef-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f6ef-108">Prerequisites</span></span>
<span data-ttu-id="1f6ef-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1f6ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f6ef-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f6ef-111">Permission type</span></span>|<span data-ttu-id="1f6ef-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f6ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f6ef-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f6ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f6ef-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f6ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f6ef-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f6ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f6ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-116">Not supported.</span></span>|
|<span data-ttu-id="1f6ef-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f6ef-117">Application</span></span>|<span data-ttu-id="1f6ef-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f6ef-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f6ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f6ef-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1f6ef-120">Optional query parameters</span></span>
<span data-ttu-id="1f6ef-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f6ef-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f6ef-122">Request headers</span></span>
|<span data-ttu-id="1f6ef-123">标头</span><span class="sxs-lookup"><span data-stu-id="1f6ef-123">Header</span></span>|<span data-ttu-id="1f6ef-124">值</span><span class="sxs-lookup"><span data-stu-id="1f6ef-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f6ef-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f6ef-125">Authorization</span></span>|<span data-ttu-id="1f6ef-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f6ef-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1f6ef-127">Accept</span></span>|<span data-ttu-id="1f6ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f6ef-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f6ef-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f6ef-129">Request body</span></span>
<span data-ttu-id="1f6ef-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f6ef-131">响应</span><span class="sxs-lookup"><span data-stu-id="1f6ef-131">Response</span></span>
<span data-ttu-id="1f6ef-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-132">If successful, this method returns a `200 OK` response code and [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f6ef-133">示例</span><span class="sxs-lookup"><span data-stu-id="1f6ef-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f6ef-134">请求</span><span class="sxs-lookup"><span data-stu-id="1f6ef-134">Request</span></span>
<span data-ttu-id="1f6ef-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="1f6ef-136">响应</span><span class="sxs-lookup"><span data-stu-id="1f6ef-136">Response</span></span>
<span data-ttu-id="1f6ef-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f6ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.locationManagementCondition",
    "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
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
}
```






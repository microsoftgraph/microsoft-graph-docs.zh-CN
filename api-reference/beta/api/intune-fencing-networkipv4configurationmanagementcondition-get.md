---
title: 获取 networkIPv4ConfigurationManagementCondition
description: 读取属性和 networkIPv4ConfigurationManagementCondition 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eb628aa17138bad6f03d96c9c9671df8339af9be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821894"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="d12da-103">获取 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d12da-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="d12da-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d12da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d12da-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d12da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d12da-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d12da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d12da-107">读取属性和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d12da-107">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d12da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d12da-108">Prerequisites</span></span>
<span data-ttu-id="d12da-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d12da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d12da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d12da-111">Permission type</span></span>|<span data-ttu-id="d12da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d12da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d12da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d12da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d12da-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d12da-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d12da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d12da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d12da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d12da-116">Not supported.</span></span>|
|<span data-ttu-id="d12da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d12da-117">Application</span></span>|<span data-ttu-id="d12da-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d12da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d12da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d12da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d12da-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d12da-120">Optional query parameters</span></span>
<span data-ttu-id="d12da-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d12da-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d12da-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d12da-122">Request headers</span></span>
|<span data-ttu-id="d12da-123">标头</span><span class="sxs-lookup"><span data-stu-id="d12da-123">Header</span></span>|<span data-ttu-id="d12da-124">值</span><span class="sxs-lookup"><span data-stu-id="d12da-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d12da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d12da-125">Authorization</span></span>|<span data-ttu-id="d12da-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d12da-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d12da-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d12da-127">Accept</span></span>|<span data-ttu-id="d12da-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d12da-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d12da-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d12da-129">Request body</span></span>
<span data-ttu-id="d12da-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d12da-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d12da-131">响应</span><span class="sxs-lookup"><span data-stu-id="d12da-131">Response</span></span>
<span data-ttu-id="d12da-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d12da-132">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d12da-133">示例</span><span class="sxs-lookup"><span data-stu-id="d12da-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d12da-134">请求</span><span class="sxs-lookup"><span data-stu-id="d12da-134">Request</span></span>
<span data-ttu-id="d12da-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d12da-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="d12da-136">响应</span><span class="sxs-lookup"><span data-stu-id="d12da-136">Response</span></span>
<span data-ttu-id="d12da-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d12da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV4Prefix": "Ip V4Prefix value",
    "ipV4Gateway": "Ip V4Gateway value",
    "ipV4DHCPServer": "Ip V4DHCPServer value",
    "ipV4DNSServerList": [
      "Ip V4DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```






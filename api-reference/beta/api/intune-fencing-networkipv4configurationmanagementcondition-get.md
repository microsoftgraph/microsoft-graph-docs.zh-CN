---
title: 获取 networkIPv4ConfigurationManagementCondition
description: 读取 networkIPv4ConfigurationManagementCondition 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6da3c71bba4babfac20e7227ac92fb83bd66939
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179913"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="8619a-103">获取 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="8619a-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="8619a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8619a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8619a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8619a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8619a-106">读取[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8619a-106">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8619a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8619a-107">Prerequisites</span></span>
<span data-ttu-id="8619a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8619a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8619a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8619a-110">Permission type</span></span>|<span data-ttu-id="8619a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8619a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8619a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8619a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8619a-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8619a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8619a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8619a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8619a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8619a-115">Not supported.</span></span>|
|<span data-ttu-id="8619a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8619a-116">Application</span></span>|<span data-ttu-id="8619a-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8619a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8619a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8619a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8619a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8619a-119">Optional query parameters</span></span>
<span data-ttu-id="8619a-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8619a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8619a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8619a-121">Request headers</span></span>
|<span data-ttu-id="8619a-122">标头</span><span class="sxs-lookup"><span data-stu-id="8619a-122">Header</span></span>|<span data-ttu-id="8619a-123">值</span><span class="sxs-lookup"><span data-stu-id="8619a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8619a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8619a-124">Authorization</span></span>|<span data-ttu-id="8619a-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8619a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8619a-126">接受</span><span class="sxs-lookup"><span data-stu-id="8619a-126">Accept</span></span>|<span data-ttu-id="8619a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8619a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8619a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8619a-128">Request body</span></span>
<span data-ttu-id="8619a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8619a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8619a-130">响应</span><span class="sxs-lookup"><span data-stu-id="8619a-130">Response</span></span>
<span data-ttu-id="8619a-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8619a-131">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8619a-132">示例</span><span class="sxs-lookup"><span data-stu-id="8619a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8619a-133">请求</span><span class="sxs-lookup"><span data-stu-id="8619a-133">Request</span></span>
<span data-ttu-id="8619a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8619a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="8619a-135">响应</span><span class="sxs-lookup"><span data-stu-id="8619a-135">Response</span></span>
<span data-ttu-id="8619a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8619a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





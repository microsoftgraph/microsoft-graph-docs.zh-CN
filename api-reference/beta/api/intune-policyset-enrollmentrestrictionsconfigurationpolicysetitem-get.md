---
title: 获取 enrollmentRestrictionsConfigurationPolicySetItem
description: 读取 enrollmentRestrictionsConfigurationPolicySetItem 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c371dfeaf9c360581ee25a0a70eb11247c28ff98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093544"
---
# <a name="get-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="0cfeb-103">获取 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="0cfeb-103">Get enrollmentRestrictionsConfigurationPolicySetItem</span></span>

<span data-ttu-id="0cfeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cfeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cfeb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cfeb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cfeb-107">读取 [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-107">Read properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cfeb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cfeb-108">Prerequisites</span></span>
<span data-ttu-id="0cfeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cfeb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cfeb-111">Permission type</span></span>|<span data-ttu-id="0cfeb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cfeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cfeb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cfeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cfeb-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cfeb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0cfeb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cfeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cfeb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-116">Not supported.</span></span>|
|<span data-ttu-id="0cfeb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cfeb-117">Application</span></span>|<span data-ttu-id="0cfeb-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cfeb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cfeb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cfeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cfeb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0cfeb-120">Optional query parameters</span></span>
<span data-ttu-id="0cfeb-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cfeb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cfeb-122">Request headers</span></span>
|<span data-ttu-id="0cfeb-123">标头</span><span class="sxs-lookup"><span data-stu-id="0cfeb-123">Header</span></span>|<span data-ttu-id="0cfeb-124">值</span><span class="sxs-lookup"><span data-stu-id="0cfeb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cfeb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cfeb-125">Authorization</span></span>|<span data-ttu-id="0cfeb-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cfeb-127">接受</span><span class="sxs-lookup"><span data-stu-id="0cfeb-127">Accept</span></span>|<span data-ttu-id="0cfeb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0cfeb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cfeb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cfeb-129">Request body</span></span>
<span data-ttu-id="0cfeb-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cfeb-131">响应</span><span class="sxs-lookup"><span data-stu-id="0cfeb-131">Response</span></span>
<span data-ttu-id="0cfeb-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-132">If successful, this method returns a `200 OK` response code and [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cfeb-133">示例</span><span class="sxs-lookup"><span data-stu-id="0cfeb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cfeb-134">请求</span><span class="sxs-lookup"><span data-stu-id="0cfeb-134">Request</span></span>
<span data-ttu-id="0cfeb-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="0cfeb-136">响应</span><span class="sxs-lookup"><span data-stu-id="0cfeb-136">Response</span></span>
<span data-ttu-id="0cfeb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cfeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
    "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ],
    "priority": 8,
    "limit": 5
  }
}
```







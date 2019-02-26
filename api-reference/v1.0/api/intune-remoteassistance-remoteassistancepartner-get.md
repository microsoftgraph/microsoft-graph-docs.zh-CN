---
title: 获取 remoteAssistancePartner
description: 读取 remoteAssistancePartner 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a796cf6ca84e3364bb2322d846bae2ccf57e754
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262830"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="49aad-103">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="49aad-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="49aad-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49aad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49aad-105">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49aad-105">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49aad-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="49aad-106">Prerequisites</span></span>
<span data-ttu-id="49aad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="49aad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49aad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49aad-109">Permission type</span></span>|<span data-ttu-id="49aad-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49aad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49aad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49aad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49aad-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="49aad-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="49aad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49aad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49aad-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49aad-114">Not supported.</span></span>|
|<span data-ttu-id="49aad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49aad-115">Application</span></span>|<span data-ttu-id="49aad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49aad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49aad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49aad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49aad-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49aad-118">Optional query parameters</span></span>
<span data-ttu-id="49aad-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="49aad-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49aad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49aad-120">Request headers</span></span>
|<span data-ttu-id="49aad-121">标头</span><span class="sxs-lookup"><span data-stu-id="49aad-121">Header</span></span>|<span data-ttu-id="49aad-122">值</span><span class="sxs-lookup"><span data-stu-id="49aad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49aad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49aad-123">Authorization</span></span>|<span data-ttu-id="49aad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49aad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49aad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49aad-125">Accept</span></span>|<span data-ttu-id="49aad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49aad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49aad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="49aad-127">Request body</span></span>
<span data-ttu-id="49aad-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49aad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49aad-129">响应</span><span class="sxs-lookup"><span data-stu-id="49aad-129">Response</span></span>
<span data-ttu-id="49aad-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49aad-130">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49aad-131">示例</span><span class="sxs-lookup"><span data-stu-id="49aad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="49aad-132">请求</span><span class="sxs-lookup"><span data-stu-id="49aad-132">Request</span></span>
<span data-ttu-id="49aad-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49aad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="49aad-134">响应</span><span class="sxs-lookup"><span data-stu-id="49aad-134">Response</span></span>
<span data-ttu-id="49aad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49aad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```




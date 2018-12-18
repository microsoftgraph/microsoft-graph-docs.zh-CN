---
title: 获取 termsAndConditionsAcceptanceStatus
description: 读取 termsAndConditionsAcceptanceStatus 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: e5e2148a1b7adfa095f065dcc6a292657765d677
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311807"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="3011b-103">获取 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="3011b-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="3011b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3011b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3011b-105">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3011b-105">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3011b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3011b-106">Prerequisites</span></span>
<span data-ttu-id="3011b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3011b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3011b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3011b-109">Permission type</span></span>|<span data-ttu-id="3011b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3011b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3011b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3011b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3011b-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3011b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3011b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3011b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3011b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3011b-114">Not supported.</span></span>|
|<span data-ttu-id="3011b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3011b-115">Application</span></span>|<span data-ttu-id="3011b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3011b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3011b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3011b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3011b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3011b-118">Optional query parameters</span></span>
<span data-ttu-id="3011b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3011b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3011b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3011b-120">Request headers</span></span>
|<span data-ttu-id="3011b-121">标头</span><span class="sxs-lookup"><span data-stu-id="3011b-121">Header</span></span>|<span data-ttu-id="3011b-122">值</span><span class="sxs-lookup"><span data-stu-id="3011b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3011b-123">授权</span><span class="sxs-lookup"><span data-stu-id="3011b-123">Authorization</span></span>|<span data-ttu-id="3011b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3011b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3011b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3011b-125">Accept</span></span>|<span data-ttu-id="3011b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3011b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3011b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3011b-127">Request body</span></span>
<span data-ttu-id="3011b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3011b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3011b-129">响应</span><span class="sxs-lookup"><span data-stu-id="3011b-129">Response</span></span>
<span data-ttu-id="3011b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3011b-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3011b-131">示例</span><span class="sxs-lookup"><span data-stu-id="3011b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3011b-132">请求</span><span class="sxs-lookup"><span data-stu-id="3011b-132">Request</span></span>
<span data-ttu-id="3011b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3011b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="3011b-134">响应</span><span class="sxs-lookup"><span data-stu-id="3011b-134">Response</span></span>
<span data-ttu-id="3011b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3011b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```




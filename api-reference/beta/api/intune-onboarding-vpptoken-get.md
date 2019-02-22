---
title: 获取 vppToken
description: 读取 vppToken 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 985bc8bc8775c55656d9feba62cc58b277113774
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153653"
---
# <a name="get-vpptoken"></a><span data-ttu-id="dd562-103">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="dd562-103">Get vppToken</span></span>

> <span data-ttu-id="dd562-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd562-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd562-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd562-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd562-106">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd562-106">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd562-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd562-107">Prerequisites</span></span>
<span data-ttu-id="dd562-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="dd562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dd562-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd562-110">Permission type</span></span>|<span data-ttu-id="dd562-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd562-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd562-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd562-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd562-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd562-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dd562-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd562-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd562-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd562-115">Not supported.</span></span>|
|<span data-ttu-id="dd562-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd562-116">Application</span></span>|<span data-ttu-id="dd562-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd562-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd562-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd562-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd562-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd562-119">Optional query parameters</span></span>
<span data-ttu-id="dd562-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd562-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd562-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd562-121">Request headers</span></span>
|<span data-ttu-id="dd562-122">标头</span><span class="sxs-lookup"><span data-stu-id="dd562-122">Header</span></span>|<span data-ttu-id="dd562-123">值</span><span class="sxs-lookup"><span data-stu-id="dd562-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd562-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd562-124">Authorization</span></span>|<span data-ttu-id="dd562-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd562-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd562-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dd562-126">Accept</span></span>|<span data-ttu-id="dd562-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd562-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd562-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd562-128">Request body</span></span>
<span data-ttu-id="dd562-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd562-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd562-130">响应</span><span class="sxs-lookup"><span data-stu-id="dd562-130">Response</span></span>
<span data-ttu-id="dd562-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd562-131">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd562-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd562-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd562-133">请求</span><span class="sxs-lookup"><span data-stu-id="dd562-133">Request</span></span>
<span data-ttu-id="dd562-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd562-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="dd562-135">响应</span><span class="sxs-lookup"><span data-stu-id="dd562-135">Response</span></span>
<span data-ttu-id="dd562-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd562-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value",
    "dataSharingConsentGranted": true,
    "displayName": "Display Name value",
    "locationName": "Location Name value",
    "claimTokenManagementFromExternalMdm": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





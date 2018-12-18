---
title: syncLicenses 操作
description: 同步与特定 appleVolumePurchaseProgramToken 关联的许可证
author: tfitzmac
ms.openlocfilehash: 541d974666988a165293f8e4241d0a15d712209a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336601"
---
# <a name="synclicenses-action"></a><span data-ttu-id="bfb84-103">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="bfb84-103">syncLicenses action</span></span>

> <span data-ttu-id="bfb84-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bfb84-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfb84-105">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="bfb84-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfb84-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfb84-106">Prerequisites</span></span>
<span data-ttu-id="bfb84-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bfb84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb84-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfb84-109">Permission type</span></span>|<span data-ttu-id="bfb84-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfb84-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfb84-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb84-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfb84-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb84-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bfb84-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb84-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfb84-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb84-114">Not supported.</span></span>|
|<span data-ttu-id="bfb84-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfb84-115">Application</span></span>|<span data-ttu-id="bfb84-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb84-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfb84-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfb84-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bfb84-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfb84-118">Request headers</span></span>
|<span data-ttu-id="bfb84-119">标头</span><span class="sxs-lookup"><span data-stu-id="bfb84-119">Header</span></span>|<span data-ttu-id="bfb84-120">值</span><span class="sxs-lookup"><span data-stu-id="bfb84-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfb84-121">授权</span><span class="sxs-lookup"><span data-stu-id="bfb84-121">Authorization</span></span>|<span data-ttu-id="bfb84-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfb84-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfb84-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bfb84-123">Accept</span></span>|<span data-ttu-id="bfb84-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bfb84-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfb84-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfb84-125">Request body</span></span>
<span data-ttu-id="bfb84-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfb84-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfb84-127">响应</span><span class="sxs-lookup"><span data-stu-id="bfb84-127">Response</span></span>
<span data-ttu-id="bfb84-128">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="bfb84-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfb84-129">示例</span><span class="sxs-lookup"><span data-stu-id="bfb84-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfb84-130">请求</span><span class="sxs-lookup"><span data-stu-id="bfb84-130">Request</span></span>
<span data-ttu-id="bfb84-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfb84-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="bfb84-132">响应</span><span class="sxs-lookup"><span data-stu-id="bfb84-132">Response</span></span>
<span data-ttu-id="bfb84-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfb84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

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
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```




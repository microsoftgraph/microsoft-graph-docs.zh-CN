---
title: syncLicenses 操作
description: 同步与特定 appleVolumePurchaseProgramToken 关联的许可证
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca8f87309c316a3fe5ed42dd6b427cd2b069efd9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254539"
---
# <a name="synclicenses-action"></a><span data-ttu-id="31151-103">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="31151-103">syncLicenses action</span></span>

> <span data-ttu-id="31151-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31151-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31151-105">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="31151-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31151-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="31151-106">Prerequisites</span></span>
<span data-ttu-id="31151-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="31151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31151-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31151-109">Permission type</span></span>|<span data-ttu-id="31151-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31151-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31151-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31151-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31151-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31151-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31151-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31151-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31151-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31151-114">Not supported.</span></span>|
|<span data-ttu-id="31151-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31151-115">Application</span></span>|<span data-ttu-id="31151-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31151-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31151-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31151-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="31151-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="31151-118">Request headers</span></span>
|<span data-ttu-id="31151-119">标头</span><span class="sxs-lookup"><span data-stu-id="31151-119">Header</span></span>|<span data-ttu-id="31151-120">值</span><span class="sxs-lookup"><span data-stu-id="31151-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31151-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31151-121">Authorization</span></span>|<span data-ttu-id="31151-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31151-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31151-123">Accept</span><span class="sxs-lookup"><span data-stu-id="31151-123">Accept</span></span>|<span data-ttu-id="31151-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31151-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31151-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="31151-125">Request body</span></span>
<span data-ttu-id="31151-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31151-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31151-127">响应</span><span class="sxs-lookup"><span data-stu-id="31151-127">Response</span></span>
<span data-ttu-id="31151-128">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="31151-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31151-129">示例</span><span class="sxs-lookup"><span data-stu-id="31151-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="31151-130">请求</span><span class="sxs-lookup"><span data-stu-id="31151-130">Request</span></span>
<span data-ttu-id="31151-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31151-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="31151-132">响应</span><span class="sxs-lookup"><span data-stu-id="31151-132">Response</span></span>
<span data-ttu-id="31151-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31151-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




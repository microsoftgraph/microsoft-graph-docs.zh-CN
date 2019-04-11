---
title: syncLicenses 操作
description: 同步与特定 appleVolumePurchaseProgramToken 关联的许可证
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 732300c26fe3e2355421f8813fd038031d5ab1e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803414"
---
# <a name="synclicenses-action"></a><span data-ttu-id="a73b1-103">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="a73b1-103">syncLicenses action</span></span>

> <span data-ttu-id="a73b1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a73b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a73b1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a73b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a73b1-106">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="a73b1-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a73b1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a73b1-107">Prerequisites</span></span>
<span data-ttu-id="a73b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a73b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73b1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a73b1-110">Permission type</span></span>|<span data-ttu-id="a73b1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a73b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a73b1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a73b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a73b1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73b1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a73b1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a73b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a73b1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a73b1-115">Not supported.</span></span>|
|<span data-ttu-id="a73b1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a73b1-116">Application</span></span>|<span data-ttu-id="a73b1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a73b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a73b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a73b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="a73b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a73b1-119">Request headers</span></span>
|<span data-ttu-id="a73b1-120">标头</span><span class="sxs-lookup"><span data-stu-id="a73b1-120">Header</span></span>|<span data-ttu-id="a73b1-121">值</span><span class="sxs-lookup"><span data-stu-id="a73b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a73b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a73b1-122">Authorization</span></span>|<span data-ttu-id="a73b1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a73b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a73b1-124">接受</span><span class="sxs-lookup"><span data-stu-id="a73b1-124">Accept</span></span>|<span data-ttu-id="a73b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a73b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a73b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a73b1-126">Request body</span></span>
<span data-ttu-id="a73b1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a73b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a73b1-128">响应</span><span class="sxs-lookup"><span data-stu-id="a73b1-128">Response</span></span>
<span data-ttu-id="a73b1-129">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="a73b1-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a73b1-130">示例</span><span class="sxs-lookup"><span data-stu-id="a73b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a73b1-131">请求</span><span class="sxs-lookup"><span data-stu-id="a73b1-131">Request</span></span>
<span data-ttu-id="a73b1-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a73b1-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="a73b1-133">响应</span><span class="sxs-lookup"><span data-stu-id="a73b1-133">Response</span></span>
<span data-ttu-id="a73b1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a73b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






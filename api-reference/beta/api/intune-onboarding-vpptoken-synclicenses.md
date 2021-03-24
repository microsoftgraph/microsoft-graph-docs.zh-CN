---
title: syncLicenses 操作
description: 同步与特定 appleVolumePurchaseProgramToken 关联的许可证
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343474868b0ae0978704186ce0ec3bd14de622a1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134982"
---
# <a name="synclicenses-action"></a><span data-ttu-id="d8589-103">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="d8589-103">syncLicenses action</span></span>

<span data-ttu-id="d8589-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8589-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8589-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8589-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8589-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8589-107">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="d8589-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8589-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8589-108">Prerequisites</span></span>
<span data-ttu-id="d8589-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8589-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8589-111">Permission type</span></span>|<span data-ttu-id="d8589-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8589-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8589-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8589-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8589-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8589-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8589-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8589-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8589-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8589-116">Not supported.</span></span>|
|<span data-ttu-id="d8589-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8589-117">Application</span></span>|<span data-ttu-id="d8589-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8589-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8589-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8589-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="d8589-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8589-120">Request headers</span></span>
|<span data-ttu-id="d8589-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8589-121">Header</span></span>|<span data-ttu-id="d8589-122">值</span><span class="sxs-lookup"><span data-stu-id="d8589-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8589-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8589-123">Authorization</span></span>|<span data-ttu-id="d8589-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8589-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8589-125">接受</span><span class="sxs-lookup"><span data-stu-id="d8589-125">Accept</span></span>|<span data-ttu-id="d8589-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8589-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8589-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8589-127">Request body</span></span>
<span data-ttu-id="d8589-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8589-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8589-129">响应</span><span class="sxs-lookup"><span data-stu-id="d8589-129">Response</span></span>
<span data-ttu-id="d8589-130">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="d8589-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8589-131">示例</span><span class="sxs-lookup"><span data-stu-id="d8589-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8589-132">请求</span><span class="sxs-lookup"><span data-stu-id="d8589-132">Request</span></span>
<span data-ttu-id="d8589-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8589-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="d8589-134">响应</span><span class="sxs-lookup"><span data-stu-id="d8589-134">Response</span></span>
<span data-ttu-id="d8589-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8589-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





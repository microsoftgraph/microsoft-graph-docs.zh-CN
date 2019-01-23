---
title: syncLicenses 操作
description: 同步与特定 appleVolumePurchaseProgramToken 关联的许可证
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79660c8de56cdf449d3fd407767bed37245ceb2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414275"
---
# <a name="synclicenses-action"></a><span data-ttu-id="b748a-103">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="b748a-103">syncLicenses action</span></span>

> <span data-ttu-id="b748a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b748a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b748a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b748a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b748a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b748a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b748a-107">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="b748a-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b748a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b748a-108">Prerequisites</span></span>
<span data-ttu-id="b748a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b748a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b748a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b748a-111">Permission type</span></span>|<span data-ttu-id="b748a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b748a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b748a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b748a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b748a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b748a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b748a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b748a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b748a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b748a-116">Not supported.</span></span>|
|<span data-ttu-id="b748a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b748a-117">Application</span></span>|<span data-ttu-id="b748a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b748a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b748a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b748a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="b748a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b748a-120">Request headers</span></span>
|<span data-ttu-id="b748a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b748a-121">Header</span></span>|<span data-ttu-id="b748a-122">值</span><span class="sxs-lookup"><span data-stu-id="b748a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b748a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b748a-123">Authorization</span></span>|<span data-ttu-id="b748a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b748a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b748a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b748a-125">Accept</span></span>|<span data-ttu-id="b748a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b748a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b748a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b748a-127">Request body</span></span>
<span data-ttu-id="b748a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b748a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b748a-129">响应</span><span class="sxs-lookup"><span data-stu-id="b748a-129">Response</span></span>
<span data-ttu-id="b748a-130">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="b748a-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b748a-131">示例</span><span class="sxs-lookup"><span data-stu-id="b748a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b748a-132">请求</span><span class="sxs-lookup"><span data-stu-id="b748a-132">Request</span></span>
<span data-ttu-id="b748a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b748a-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="b748a-134">响应</span><span class="sxs-lookup"><span data-stu-id="b748a-134">Response</span></span>
<span data-ttu-id="b748a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b748a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





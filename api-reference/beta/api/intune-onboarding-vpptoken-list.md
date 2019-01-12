---
title: 列出 vppTokens
description: 列出 vppToken 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 993e7f8917ed60185159303dffc2be957816d4c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976192"
---
# <a name="list-vpptokens"></a><span data-ttu-id="1e6f8-103">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="1e6f8-103">List vppTokens</span></span>

> <span data-ttu-id="1e6f8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e6f8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e6f8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e6f8-107">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-107">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e6f8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e6f8-108">Prerequisites</span></span>
<span data-ttu-id="1e6f8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1e6f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e6f8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e6f8-111">Permission type</span></span>|<span data-ttu-id="1e6f8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e6f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e6f8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e6f8-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e6f8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1e6f8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e6f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-116">Not supported.</span></span>|
|<span data-ttu-id="1e6f8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e6f8-117">Application</span></span>|<span data-ttu-id="1e6f8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e6f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e6f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="1e6f8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e6f8-120">Request headers</span></span>
|<span data-ttu-id="1e6f8-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e6f8-121">Header</span></span>|<span data-ttu-id="1e6f8-122">值</span><span class="sxs-lookup"><span data-stu-id="1e6f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e6f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e6f8-123">Authorization</span></span>|<span data-ttu-id="1e6f8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e6f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e6f8-125">Accept</span></span>|<span data-ttu-id="1e6f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e6f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e6f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e6f8-127">Request body</span></span>
<span data-ttu-id="1e6f8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e6f8-129">响应</span><span class="sxs-lookup"><span data-stu-id="1e6f8-129">Response</span></span>
<span data-ttu-id="1e6f8-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-130">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e6f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e6f8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e6f8-132">请求</span><span class="sxs-lookup"><span data-stu-id="1e6f8-132">Request</span></span>
<span data-ttu-id="1e6f8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="1e6f8-134">响应</span><span class="sxs-lookup"><span data-stu-id="1e6f8-134">Response</span></span>
<span data-ttu-id="1e6f8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e6f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1190

{
  "value": [
    {
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
      "claimTokenManagementFromExternalMdm": true
    }
  ]
}
```






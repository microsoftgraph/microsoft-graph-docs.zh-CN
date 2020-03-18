---
title: 列出 deviceManagementDerivedCredentialSettingses
description: 列出 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5a9af858fd5b1c2d19458abe4a733660d5f12a2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801003"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="9390a-103">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="9390a-103">List deviceManagementDerivedCredentialSettingses</span></span>

> <span data-ttu-id="9390a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9390a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9390a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9390a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9390a-106">列出[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9390a-106">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9390a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9390a-107">Prerequisites</span></span>
<span data-ttu-id="9390a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9390a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9390a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9390a-110">Permission type</span></span>|<span data-ttu-id="9390a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9390a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9390a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9390a-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="9390a-113">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="9390a-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="9390a-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9390a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9390a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9390a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9390a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9390a-116">Not supported.</span></span>|
|<span data-ttu-id="9390a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9390a-117">Application</span></span>||
|<span data-ttu-id="9390a-118">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="9390a-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="9390a-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9390a-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9390a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9390a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="9390a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9390a-121">Request headers</span></span>
|<span data-ttu-id="9390a-122">标头</span><span class="sxs-lookup"><span data-stu-id="9390a-122">Header</span></span>|<span data-ttu-id="9390a-123">值</span><span class="sxs-lookup"><span data-stu-id="9390a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9390a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9390a-124">Authorization</span></span>|<span data-ttu-id="9390a-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9390a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9390a-126">接受</span><span class="sxs-lookup"><span data-stu-id="9390a-126">Accept</span></span>|<span data-ttu-id="9390a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9390a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9390a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9390a-128">Request body</span></span>
<span data-ttu-id="9390a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9390a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9390a-130">响应</span><span class="sxs-lookup"><span data-stu-id="9390a-130">Response</span></span>
<span data-ttu-id="9390a-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9390a-131">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9390a-132">示例</span><span class="sxs-lookup"><span data-stu-id="9390a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9390a-133">请求</span><span class="sxs-lookup"><span data-stu-id="9390a-133">Request</span></span>
<span data-ttu-id="9390a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9390a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="9390a-135">响应</span><span class="sxs-lookup"><span data-stu-id="9390a-135">Response</span></span>
<span data-ttu-id="9390a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9390a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```









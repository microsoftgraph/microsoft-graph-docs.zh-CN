---
title: 列出 windowsAutopilotDeploymentProfilePolicySetItems
description: 列出 windowsAutopilotDeploymentProfilePolicySetItem 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b194cde6c55e8bcb2fd041dfe06567d90ab2cbb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537315"
---
# <a name="list-windowsautopilotdeploymentprofilepolicysetitems"></a><span data-ttu-id="7c214-103">列出 windowsAutopilotDeploymentProfilePolicySetItems</span><span class="sxs-lookup"><span data-stu-id="7c214-103">List windowsAutopilotDeploymentProfilePolicySetItems</span></span>

> <span data-ttu-id="7c214-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c214-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c214-106">列出[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c214-106">List properties and relationships of the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c214-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c214-107">Prerequisites</span></span>
<span data-ttu-id="7c214-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c214-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c214-110">Permission type</span></span>|<span data-ttu-id="7c214-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7c214-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c214-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c214-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c214-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c214-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c214-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c214-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c214-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c214-115">Not supported.</span></span>|
|<span data-ttu-id="7c214-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c214-116">Application</span></span>|<span data-ttu-id="7c214-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c214-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c214-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c214-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="7c214-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c214-119">Request headers</span></span>
|<span data-ttu-id="7c214-120">标头</span><span class="sxs-lookup"><span data-stu-id="7c214-120">Header</span></span>|<span data-ttu-id="7c214-121">值</span><span class="sxs-lookup"><span data-stu-id="7c214-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c214-122">授权</span><span class="sxs-lookup"><span data-stu-id="7c214-122">Authorization</span></span>|<span data-ttu-id="7c214-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c214-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c214-124">接受</span><span class="sxs-lookup"><span data-stu-id="7c214-124">Accept</span></span>|<span data-ttu-id="7c214-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c214-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c214-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c214-126">Request body</span></span>
<span data-ttu-id="7c214-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c214-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c214-128">响应</span><span class="sxs-lookup"><span data-stu-id="7c214-128">Response</span></span>
<span data-ttu-id="7c214-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7c214-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c214-130">示例</span><span class="sxs-lookup"><span data-stu-id="7c214-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c214-131">请求</span><span class="sxs-lookup"><span data-stu-id="7c214-131">Request</span></span>
<span data-ttu-id="7c214-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c214-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="7c214-133">响应</span><span class="sxs-lookup"><span data-stu-id="7c214-133">Response</span></span>
<span data-ttu-id="7c214-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c214-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
      "id": "850e84d8-84d8-850e-d884-0e85d8840e85",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```







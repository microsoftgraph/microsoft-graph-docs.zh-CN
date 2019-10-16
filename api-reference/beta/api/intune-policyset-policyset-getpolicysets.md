---
title: getPolicySets 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 815c49c6886d22dce0c612f7178acd73ccd9ea07
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536327"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="4a313-103">getPolicySets 操作</span><span class="sxs-lookup"><span data-stu-id="4a313-103">getPolicySets action</span></span>

> <span data-ttu-id="4a313-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a313-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a313-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a313-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a313-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4a313-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a313-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a313-107">Prerequisites</span></span>
<span data-ttu-id="4a313-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a313-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a313-110">Permission type</span></span>|<span data-ttu-id="4a313-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a313-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a313-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a313-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a313-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a313-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a313-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a313-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a313-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a313-115">Not supported.</span></span>|
|<span data-ttu-id="4a313-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a313-116">Application</span></span>|<span data-ttu-id="4a313-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a313-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a313-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a313-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="4a313-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a313-119">Request headers</span></span>
|<span data-ttu-id="4a313-120">标头</span><span class="sxs-lookup"><span data-stu-id="4a313-120">Header</span></span>|<span data-ttu-id="4a313-121">值</span><span class="sxs-lookup"><span data-stu-id="4a313-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a313-122">授权</span><span class="sxs-lookup"><span data-stu-id="4a313-122">Authorization</span></span>|<span data-ttu-id="4a313-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a313-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a313-124">接受</span><span class="sxs-lookup"><span data-stu-id="4a313-124">Accept</span></span>|<span data-ttu-id="4a313-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a313-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a313-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a313-126">Request body</span></span>
<span data-ttu-id="4a313-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a313-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4a313-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4a313-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4a313-129">属性</span><span class="sxs-lookup"><span data-stu-id="4a313-129">Property</span></span>|<span data-ttu-id="4a313-130">类型</span><span class="sxs-lookup"><span data-stu-id="4a313-130">Type</span></span>|<span data-ttu-id="4a313-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a313-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a313-132">policySetIds</span><span class="sxs-lookup"><span data-stu-id="4a313-132">policySetIds</span></span>|<span data-ttu-id="4a313-133">String collection</span><span class="sxs-lookup"><span data-stu-id="4a313-133">String collection</span></span>|<span data-ttu-id="4a313-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4a313-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a313-135">响应</span><span class="sxs-lookup"><span data-stu-id="4a313-135">Response</span></span>
<span data-ttu-id="4a313-136">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[policySet](../resources/intune-policyset-policyset.md)集合。</span><span class="sxs-lookup"><span data-stu-id="4a313-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a313-137">示例</span><span class="sxs-lookup"><span data-stu-id="4a313-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a313-138">请求</span><span class="sxs-lookup"><span data-stu-id="4a313-138">Request</span></span>
<span data-ttu-id="4a313-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a313-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/getPolicySets

Content-type: application/json
Content-length: 58

{
  "policySetIds": [
    "Policy Set Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4a313-140">响应</span><span class="sxs-lookup"><span data-stu-id="4a313-140">Response</span></span>
<span data-ttu-id="4a313-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a313-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "653cb373-b373-653c-73b3-3c6573b33c65",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "roleScopeTags": [
        "Role Scope Tags value"
      ]
    }
  ]
}
```







---
title: 列出 securityBaselineTemplates
description: 列出 securityBaselineTemplate 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d13ea42549f3244720bfac6bb8ff1be93e6914f0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531929"
---
# <a name="list-securitybaselinetemplates"></a><span data-ttu-id="f4df2-103">列出 securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="f4df2-103">List securityBaselineTemplates</span></span>

> <span data-ttu-id="f4df2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4df2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4df2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4df2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4df2-106">列出[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4df2-106">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4df2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4df2-107">Prerequisites</span></span>
<span data-ttu-id="f4df2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4df2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4df2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4df2-110">Permission type</span></span>|<span data-ttu-id="f4df2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4df2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4df2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4df2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4df2-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4df2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f4df2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4df2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4df2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4df2-115">Not supported.</span></span>|
|<span data-ttu-id="f4df2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4df2-116">Application</span></span>|<span data-ttu-id="f4df2-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4df2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4df2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4df2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="f4df2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4df2-119">Request headers</span></span>
|<span data-ttu-id="f4df2-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4df2-120">Header</span></span>|<span data-ttu-id="f4df2-121">值</span><span class="sxs-lookup"><span data-stu-id="f4df2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4df2-122">授权</span><span class="sxs-lookup"><span data-stu-id="f4df2-122">Authorization</span></span>|<span data-ttu-id="f4df2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4df2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4df2-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4df2-124">Accept</span></span>|<span data-ttu-id="f4df2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4df2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4df2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4df2-126">Request body</span></span>
<span data-ttu-id="f4df2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4df2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4df2-128">响应</span><span class="sxs-lookup"><span data-stu-id="f4df2-128">Response</span></span>
<span data-ttu-id="f4df2-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4df2-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4df2-130">示例</span><span class="sxs-lookup"><span data-stu-id="f4df2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4df2-131">请求</span><span class="sxs-lookup"><span data-stu-id="f4df2-131">Request</span></span>
<span data-ttu-id="f4df2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4df2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="f4df2-133">响应</span><span class="sxs-lookup"><span data-stu-id="f4df2-133">Response</span></span>
<span data-ttu-id="f4df2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4df2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineTemplate",
      "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "specializedDevices",
      "platformType": "androidForWork",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```







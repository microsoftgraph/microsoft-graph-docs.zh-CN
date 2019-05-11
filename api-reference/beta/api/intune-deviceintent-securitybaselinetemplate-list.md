---
title: 列出 securityBaselineTemplates
description: 列出 securityBaselineTemplate 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6276cfe94eac8db637ce50738dc27e667f1106f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33911684"
---
# <a name="list-securitybaselinetemplates"></a><span data-ttu-id="ca5ad-103">列出 securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="ca5ad-103">List securityBaselineTemplates</span></span>

> <span data-ttu-id="ca5ad-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca5ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca5ad-106">列出[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-106">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca5ad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca5ad-107">Prerequisites</span></span>
<span data-ttu-id="ca5ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca5ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca5ad-110">Permission type</span></span>|<span data-ttu-id="ca5ad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca5ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca5ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca5ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca5ad-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca5ad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca5ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca5ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca5ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-115">Not supported.</span></span>|
|<span data-ttu-id="ca5ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca5ad-116">Application</span></span>|<span data-ttu-id="ca5ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca5ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca5ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="ca5ad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca5ad-119">Request headers</span></span>
|<span data-ttu-id="ca5ad-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca5ad-120">Header</span></span>|<span data-ttu-id="ca5ad-121">值</span><span class="sxs-lookup"><span data-stu-id="ca5ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca5ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca5ad-122">Authorization</span></span>|<span data-ttu-id="ca5ad-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca5ad-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca5ad-124">Accept</span></span>|<span data-ttu-id="ca5ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca5ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca5ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca5ad-126">Request body</span></span>
<span data-ttu-id="ca5ad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca5ad-128">响应</span><span class="sxs-lookup"><span data-stu-id="ca5ad-128">Response</span></span>
<span data-ttu-id="ca5ad-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca5ad-130">示例</span><span class="sxs-lookup"><span data-stu-id="ca5ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca5ad-131">请求</span><span class="sxs-lookup"><span data-stu-id="ca5ad-131">Request</span></span>
<span data-ttu-id="ca5ad-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="ca5ad-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca5ad-133">Response</span></span>
<span data-ttu-id="ca5ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca5ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineTemplate",
      "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11
    }
  ]
}
```





---
title: getAuditCategories 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cbd84df96c898daa8586920eac73b9a36813710
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757466"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="effad-103">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="effad-103">getAuditCategories function</span></span>

<span data-ttu-id="effad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="effad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="effad-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="effad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="effad-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="effad-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="effad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="effad-107">Prerequisites</span></span>
<span data-ttu-id="effad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="effad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="effad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="effad-110">Permission type</span></span>|<span data-ttu-id="effad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="effad-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="effad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="effad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="effad-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effad-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="effad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="effad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="effad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="effad-115">Not supported.</span></span>|
|<span data-ttu-id="effad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="effad-116">Application</span></span>|<span data-ttu-id="effad-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effad-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="effad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="effad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="effad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="effad-119">Request headers</span></span>
|<span data-ttu-id="effad-120">标头</span><span class="sxs-lookup"><span data-stu-id="effad-120">Header</span></span>|<span data-ttu-id="effad-121">值</span><span class="sxs-lookup"><span data-stu-id="effad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="effad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="effad-122">Authorization</span></span>|<span data-ttu-id="effad-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="effad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="effad-124">接受</span><span class="sxs-lookup"><span data-stu-id="effad-124">Accept</span></span>|<span data-ttu-id="effad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="effad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="effad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="effad-126">Request body</span></span>
<span data-ttu-id="effad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="effad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="effad-128">响应</span><span class="sxs-lookup"><span data-stu-id="effad-128">Response</span></span>
<span data-ttu-id="effad-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="effad-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="effad-130">示例</span><span class="sxs-lookup"><span data-stu-id="effad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="effad-131">请求</span><span class="sxs-lookup"><span data-stu-id="effad-131">Request</span></span>
<span data-ttu-id="effad-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="effad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="effad-133">响应</span><span class="sxs-lookup"><span data-stu-id="effad-133">Response</span></span>
<span data-ttu-id="effad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="effad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```





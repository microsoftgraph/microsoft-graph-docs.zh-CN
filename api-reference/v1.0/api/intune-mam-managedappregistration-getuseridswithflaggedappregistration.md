---
title: getUserIdsWithFlaggedAppRegistration 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf68ce2707d772eec15729c564e7259a3835ef50
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43398666"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="80cf3-103">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="80cf3-103">getUserIdsWithFlaggedAppRegistration function</span></span>

<span data-ttu-id="80cf3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80cf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80cf3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80cf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80cf3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="80cf3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80cf3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="80cf3-107">Prerequisites</span></span>
<span data-ttu-id="80cf3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80cf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80cf3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80cf3-110">Permission type</span></span>|<span data-ttu-id="80cf3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80cf3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80cf3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80cf3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80cf3-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="80cf3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="80cf3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80cf3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80cf3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80cf3-115">Not supported.</span></span>|
|<span data-ttu-id="80cf3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80cf3-116">Application</span></span>|<span data-ttu-id="80cf3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="80cf3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80cf3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80cf3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="80cf3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="80cf3-119">Request headers</span></span>
|<span data-ttu-id="80cf3-120">标头</span><span class="sxs-lookup"><span data-stu-id="80cf3-120">Header</span></span>|<span data-ttu-id="80cf3-121">值</span><span class="sxs-lookup"><span data-stu-id="80cf3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80cf3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80cf3-122">Authorization</span></span>|<span data-ttu-id="80cf3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80cf3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80cf3-124">接受</span><span class="sxs-lookup"><span data-stu-id="80cf3-124">Accept</span></span>|<span data-ttu-id="80cf3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80cf3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80cf3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="80cf3-126">Request body</span></span>
<span data-ttu-id="80cf3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80cf3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80cf3-128">响应</span><span class="sxs-lookup"><span data-stu-id="80cf3-128">Response</span></span>
<span data-ttu-id="80cf3-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="80cf3-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80cf3-130">示例</span><span class="sxs-lookup"><span data-stu-id="80cf3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="80cf3-131">请求</span><span class="sxs-lookup"><span data-stu-id="80cf3-131">Request</span></span>
<span data-ttu-id="80cf3-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80cf3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="80cf3-133">响应</span><span class="sxs-lookup"><span data-stu-id="80cf3-133">Response</span></span>
<span data-ttu-id="80cf3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80cf3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```







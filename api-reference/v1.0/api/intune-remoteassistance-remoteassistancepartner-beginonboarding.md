---
title: beginOnboarding 操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d16b7f89470c50fa50c5c6cb37a6792a5995ee9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361677"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="21d92-103">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="21d92-103">beginOnboarding action</span></span>

> <span data-ttu-id="21d92-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21d92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d92-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21d92-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21d92-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="21d92-106">Prerequisites</span></span>
<span data-ttu-id="21d92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21d92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21d92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="21d92-109">Permission type</span></span>|<span data-ttu-id="21d92-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21d92-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21d92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21d92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21d92-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d92-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21d92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21d92-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21d92-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="21d92-114">Not supported.</span></span>|
|<span data-ttu-id="21d92-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="21d92-115">Application</span></span>|<span data-ttu-id="21d92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21d92-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21d92-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21d92-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="21d92-118">请求头</span><span class="sxs-lookup"><span data-stu-id="21d92-118">Request headers</span></span>
|<span data-ttu-id="21d92-119">标头</span><span class="sxs-lookup"><span data-stu-id="21d92-119">Header</span></span>|<span data-ttu-id="21d92-120">值</span><span class="sxs-lookup"><span data-stu-id="21d92-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21d92-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21d92-121">Authorization</span></span>|<span data-ttu-id="21d92-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21d92-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21d92-123">接受</span><span class="sxs-lookup"><span data-stu-id="21d92-123">Accept</span></span>|<span data-ttu-id="21d92-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21d92-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21d92-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="21d92-125">Request body</span></span>
<span data-ttu-id="21d92-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21d92-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21d92-127">响应</span><span class="sxs-lookup"><span data-stu-id="21d92-127">Response</span></span>
<span data-ttu-id="21d92-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="21d92-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="21d92-129">示例</span><span class="sxs-lookup"><span data-stu-id="21d92-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="21d92-130">请求</span><span class="sxs-lookup"><span data-stu-id="21d92-130">Request</span></span>
<span data-ttu-id="21d92-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21d92-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="21d92-132">响应</span><span class="sxs-lookup"><span data-stu-id="21d92-132">Response</span></span>
<span data-ttu-id="21d92-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21d92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f485349a2bcf9b69eee428e98be39bce7bb5f50f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361565"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="c94dc-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="c94dc-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="c94dc-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c94dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c94dc-105">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="c94dc-105">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c94dc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c94dc-106">Prerequisites</span></span>
<span data-ttu-id="c94dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c94dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c94dc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c94dc-109">Permission type</span></span>|<span data-ttu-id="c94dc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c94dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c94dc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c94dc-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="c94dc-112">&nbsp; &nbsp; _载入_</span><span class="sxs-lookup"><span data-stu-id="c94dc-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="c94dc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94dc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c94dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c94dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c94dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c94dc-115">Not supported.</span></span>|
|<span data-ttu-id="c94dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c94dc-116">Application</span></span>|<span data-ttu-id="c94dc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c94dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c94dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c94dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="c94dc-119">请求头</span><span class="sxs-lookup"><span data-stu-id="c94dc-119">Request headers</span></span>
|<span data-ttu-id="c94dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="c94dc-120">Header</span></span>|<span data-ttu-id="c94dc-121">值</span><span class="sxs-lookup"><span data-stu-id="c94dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c94dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c94dc-122">Authorization</span></span>|<span data-ttu-id="c94dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c94dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c94dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="c94dc-124">Accept</span></span>|<span data-ttu-id="c94dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c94dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c94dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c94dc-126">Request body</span></span>
<span data-ttu-id="c94dc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c94dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c94dc-128">响应</span><span class="sxs-lookup"><span data-stu-id="c94dc-128">Response</span></span>
<span data-ttu-id="c94dc-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c94dc-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="c94dc-130">示例请求</span><span class="sxs-lookup"><span data-stu-id="c94dc-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="c94dc-131">响应</span><span class="sxs-lookup"><span data-stu-id="c94dc-131">Response</span></span>

<span data-ttu-id="c94dc-132">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c94dc-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c94dc-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c94dc-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```





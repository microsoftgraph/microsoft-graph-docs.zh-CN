---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba25378dae6f74104cb3ecc3a336404181b9a79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821642"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="41ffa-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="41ffa-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="41ffa-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41ffa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41ffa-105">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="41ffa-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41ffa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="41ffa-106">Prerequisites</span></span>
<span data-ttu-id="41ffa-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="41ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41ffa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="41ffa-109">Permission type</span></span>|<span data-ttu-id="41ffa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41ffa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41ffa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41ffa-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="41ffa-112">&nbsp;&nbsp; _入职培训_</span><span class="sxs-lookup"><span data-stu-id="41ffa-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="41ffa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ffa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41ffa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41ffa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41ffa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41ffa-115">Not supported.</span></span>|
|<span data-ttu-id="41ffa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41ffa-116">Application</span></span>|<span data-ttu-id="41ffa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41ffa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41ffa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41ffa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="41ffa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41ffa-119">Request headers</span></span>
|<span data-ttu-id="41ffa-120">标头</span><span class="sxs-lookup"><span data-stu-id="41ffa-120">Header</span></span>|<span data-ttu-id="41ffa-121">值</span><span class="sxs-lookup"><span data-stu-id="41ffa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41ffa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41ffa-122">Authorization</span></span>|<span data-ttu-id="41ffa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41ffa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41ffa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41ffa-124">Accept</span></span>|<span data-ttu-id="41ffa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41ffa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41ffa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41ffa-126">Request body</span></span>
<span data-ttu-id="41ffa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41ffa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41ffa-128">响应</span><span class="sxs-lookup"><span data-stu-id="41ffa-128">Response</span></span>
<span data-ttu-id="41ffa-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="41ffa-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="41ffa-130">示例请求</span><span class="sxs-lookup"><span data-stu-id="41ffa-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="41ffa-131">响应</span><span class="sxs-lookup"><span data-stu-id="41ffa-131">Response</span></span>

<span data-ttu-id="41ffa-132">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="41ffa-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="41ffa-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41ffa-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




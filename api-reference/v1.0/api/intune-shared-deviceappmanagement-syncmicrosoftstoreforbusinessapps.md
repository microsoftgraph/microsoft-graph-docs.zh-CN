---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: tfitzmac
ms.openlocfilehash: b26b379631cf5b28594e3cf247b735d6118e9b40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354332"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="0af6e-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="0af6e-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="0af6e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0af6e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0af6e-105">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="0af6e-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0af6e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0af6e-106">Prerequisites</span></span>
<span data-ttu-id="0af6e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0af6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af6e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0af6e-109">Permission type</span></span>|<span data-ttu-id="0af6e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0af6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0af6e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0af6e-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="0af6e-112">&nbsp;&nbsp; _入职培训_</span><span class="sxs-lookup"><span data-stu-id="0af6e-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="0af6e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af6e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0af6e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0af6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0af6e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af6e-115">Not supported.</span></span>|
|<span data-ttu-id="0af6e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0af6e-116">Application</span></span>|<span data-ttu-id="0af6e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af6e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0af6e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0af6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="0af6e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0af6e-119">Request headers</span></span>
|<span data-ttu-id="0af6e-120">标头</span><span class="sxs-lookup"><span data-stu-id="0af6e-120">Header</span></span>|<span data-ttu-id="0af6e-121">值</span><span class="sxs-lookup"><span data-stu-id="0af6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0af6e-122">授权</span><span class="sxs-lookup"><span data-stu-id="0af6e-122">Authorization</span></span>|<span data-ttu-id="0af6e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0af6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0af6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0af6e-124">Accept</span></span>|<span data-ttu-id="0af6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0af6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af6e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0af6e-126">Request body</span></span>
<span data-ttu-id="0af6e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0af6e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0af6e-128">响应</span><span class="sxs-lookup"><span data-stu-id="0af6e-128">Response</span></span>
<span data-ttu-id="0af6e-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0af6e-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="0af6e-130">示例请求</span><span class="sxs-lookup"><span data-stu-id="0af6e-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="0af6e-131">响应</span><span class="sxs-lookup"><span data-stu-id="0af6e-131">Response</span></span>

<span data-ttu-id="0af6e-132">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="0af6e-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0af6e-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0af6e-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




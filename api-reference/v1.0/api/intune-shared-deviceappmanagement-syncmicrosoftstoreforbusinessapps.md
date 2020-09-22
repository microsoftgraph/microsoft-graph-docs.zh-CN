---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a9deb0ab2e84a4debf11040010bc65fad01f65b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019248"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="1b9e6-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="1b9e6-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="1b9e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b9e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b9e6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b9e6-106">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="1b9e6-106">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b9e6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b9e6-107">Prerequisites</span></span>
<span data-ttu-id="1b9e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b9e6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b9e6-110">Permission type</span></span>|<span data-ttu-id="1b9e6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b9e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b9e6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b9e6-112">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="1b9e6-113">&nbsp; &nbsp; _载入_</span><span class="sxs-lookup"><span data-stu-id="1b9e6-113">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="1b9e6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b9e6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b9e6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b9e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b9e6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-116">Not supported.</span></span>|
|<span data-ttu-id="1b9e6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b9e6-117">Application</span></span>|<span data-ttu-id="1b9e6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b9e6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b9e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="1b9e6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b9e6-120">Request headers</span></span>
|<span data-ttu-id="1b9e6-121">标头</span><span class="sxs-lookup"><span data-stu-id="1b9e6-121">Header</span></span>|<span data-ttu-id="1b9e6-122">值</span><span class="sxs-lookup"><span data-stu-id="1b9e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b9e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b9e6-123">Authorization</span></span>|<span data-ttu-id="1b9e6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b9e6-125">接受</span><span class="sxs-lookup"><span data-stu-id="1b9e6-125">Accept</span></span>|<span data-ttu-id="1b9e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b9e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b9e6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b9e6-127">Request body</span></span>
<span data-ttu-id="1b9e6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b9e6-129">响应</span><span class="sxs-lookup"><span data-stu-id="1b9e6-129">Response</span></span>
<span data-ttu-id="1b9e6-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="1b9e6-131">示例请求</span><span class="sxs-lookup"><span data-stu-id="1b9e6-131">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="1b9e6-132">响应</span><span class="sxs-lookup"><span data-stu-id="1b9e6-132">Response</span></span>

<span data-ttu-id="1b9e6-133">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-133">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1b9e6-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b9e6-134">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










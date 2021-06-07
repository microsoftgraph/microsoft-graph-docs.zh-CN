---
title: beginOnboarding 操作
description: 开始载入的请求。  必须与相应的 TeamViewer 帐户信息结合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc4285513e9ea847bee5014aeab6e62afd8d6f17
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759035"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="efc89-104">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="efc89-104">beginOnboarding action</span></span>

<span data-ttu-id="efc89-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efc89-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efc89-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efc89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efc89-107">开始载入的请求。</span><span class="sxs-lookup"><span data-stu-id="efc89-107">A request to start onboarding.</span></span>  <span data-ttu-id="efc89-108">必须与相应的 TeamViewer 帐户信息结合</span><span class="sxs-lookup"><span data-stu-id="efc89-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efc89-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="efc89-109">Prerequisites</span></span>
<span data-ttu-id="efc89-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efc89-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efc89-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="efc89-112">Permission type</span></span>|<span data-ttu-id="efc89-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efc89-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efc89-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efc89-114">Delegated (work or school account)</span></span>|<span data-ttu-id="efc89-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efc89-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efc89-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efc89-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efc89-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="efc89-117">Not supported.</span></span>|
|<span data-ttu-id="efc89-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="efc89-118">Application</span></span>|<span data-ttu-id="efc89-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efc89-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efc89-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efc89-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="efc89-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="efc89-121">Request headers</span></span>
|<span data-ttu-id="efc89-122">标头</span><span class="sxs-lookup"><span data-stu-id="efc89-122">Header</span></span>|<span data-ttu-id="efc89-123">值</span><span class="sxs-lookup"><span data-stu-id="efc89-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efc89-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="efc89-124">Authorization</span></span>|<span data-ttu-id="efc89-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efc89-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efc89-126">接受</span><span class="sxs-lookup"><span data-stu-id="efc89-126">Accept</span></span>|<span data-ttu-id="efc89-127">application/json</span><span class="sxs-lookup"><span data-stu-id="efc89-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efc89-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="efc89-128">Request body</span></span>
<span data-ttu-id="efc89-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efc89-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efc89-130">响应</span><span class="sxs-lookup"><span data-stu-id="efc89-130">Response</span></span>
<span data-ttu-id="efc89-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="efc89-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efc89-132">示例</span><span class="sxs-lookup"><span data-stu-id="efc89-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="efc89-133">请求</span><span class="sxs-lookup"><span data-stu-id="efc89-133">Request</span></span>
<span data-ttu-id="efc89-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efc89-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="efc89-135">响应</span><span class="sxs-lookup"><span data-stu-id="efc89-135">Response</span></span>
<span data-ttu-id="efc89-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efc89-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





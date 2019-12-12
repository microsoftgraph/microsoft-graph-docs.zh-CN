---
title: beginOnboarding 操作
description: 启动 "加入" 的请求。  必须与相应的 TeamViewer 帐户信息结合使用
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f115502c8f0197eeccfb68f69c443570cd6bbc9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955131"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="76e69-104">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="76e69-104">beginOnboarding action</span></span>

> <span data-ttu-id="76e69-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76e69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76e69-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76e69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76e69-107">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="76e69-107">A request to start onboarding.</span></span>  <span data-ttu-id="76e69-108">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="76e69-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76e69-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="76e69-109">Prerequisites</span></span>
<span data-ttu-id="76e69-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76e69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e69-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="76e69-112">Permission type</span></span>|<span data-ttu-id="76e69-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76e69-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76e69-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76e69-114">Delegated (work or school account)</span></span>|<span data-ttu-id="76e69-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e69-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="76e69-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76e69-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76e69-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="76e69-117">Not supported.</span></span>|
|<span data-ttu-id="76e69-118">Application</span><span class="sxs-lookup"><span data-stu-id="76e69-118">Application</span></span>|<span data-ttu-id="76e69-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e69-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76e69-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76e69-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="76e69-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="76e69-121">Request headers</span></span>
|<span data-ttu-id="76e69-122">标头</span><span class="sxs-lookup"><span data-stu-id="76e69-122">Header</span></span>|<span data-ttu-id="76e69-123">值</span><span class="sxs-lookup"><span data-stu-id="76e69-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76e69-124">授权</span><span class="sxs-lookup"><span data-stu-id="76e69-124">Authorization</span></span>|<span data-ttu-id="76e69-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76e69-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76e69-126">接受</span><span class="sxs-lookup"><span data-stu-id="76e69-126">Accept</span></span>|<span data-ttu-id="76e69-127">application/json</span><span class="sxs-lookup"><span data-stu-id="76e69-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e69-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="76e69-128">Request body</span></span>
<span data-ttu-id="76e69-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76e69-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76e69-130">响应</span><span class="sxs-lookup"><span data-stu-id="76e69-130">Response</span></span>
<span data-ttu-id="76e69-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="76e69-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76e69-132">示例</span><span class="sxs-lookup"><span data-stu-id="76e69-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="76e69-133">请求</span><span class="sxs-lookup"><span data-stu-id="76e69-133">Request</span></span>
<span data-ttu-id="76e69-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76e69-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="76e69-135">响应</span><span class="sxs-lookup"><span data-stu-id="76e69-135">Response</span></span>
<span data-ttu-id="76e69-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76e69-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






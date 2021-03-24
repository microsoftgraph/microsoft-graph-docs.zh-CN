---
title: beginOnboarding 操作
description: 开始载入的请求。  必须与相应的 TeamViewer 帐户信息结合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4ffc6dc5ded86e7007c3a3b87fdd2007c792eab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134464"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="dbf3f-104">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="dbf3f-104">beginOnboarding action</span></span>

<span data-ttu-id="dbf3f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbf3f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbf3f-106">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbf3f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf3f-108">开始载入的请求。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-108">A request to start onboarding.</span></span>  <span data-ttu-id="dbf3f-109">必须与相应的 TeamViewer 帐户信息结合</span><span class="sxs-lookup"><span data-stu-id="dbf3f-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbf3f-110">先决条件</span><span class="sxs-lookup"><span data-stu-id="dbf3f-110">Prerequisites</span></span>
<span data-ttu-id="dbf3f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbf3f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbf3f-113">Permission type</span></span>|<span data-ttu-id="dbf3f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbf3f-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbf3f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf3f-115">Delegated (work or school account)</span></span>|<span data-ttu-id="dbf3f-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf3f-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dbf3f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf3f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbf3f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-118">Not supported.</span></span>|
|<span data-ttu-id="dbf3f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbf3f-119">Application</span></span>|<span data-ttu-id="dbf3f-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf3f-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbf3f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbf3f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="dbf3f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbf3f-122">Request headers</span></span>
|<span data-ttu-id="dbf3f-123">标头</span><span class="sxs-lookup"><span data-stu-id="dbf3f-123">Header</span></span>|<span data-ttu-id="dbf3f-124">值</span><span class="sxs-lookup"><span data-stu-id="dbf3f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbf3f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbf3f-125">Authorization</span></span>|<span data-ttu-id="dbf3f-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbf3f-127">接受</span><span class="sxs-lookup"><span data-stu-id="dbf3f-127">Accept</span></span>|<span data-ttu-id="dbf3f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dbf3f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbf3f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbf3f-129">Request body</span></span>
<span data-ttu-id="dbf3f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbf3f-131">响应</span><span class="sxs-lookup"><span data-stu-id="dbf3f-131">Response</span></span>
<span data-ttu-id="dbf3f-132">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dbf3f-133">示例</span><span class="sxs-lookup"><span data-stu-id="dbf3f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbf3f-134">请求</span><span class="sxs-lookup"><span data-stu-id="dbf3f-134">Request</span></span>
<span data-ttu-id="dbf3f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="dbf3f-136">响应</span><span class="sxs-lookup"><span data-stu-id="dbf3f-136">Response</span></span>
<span data-ttu-id="dbf3f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbf3f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





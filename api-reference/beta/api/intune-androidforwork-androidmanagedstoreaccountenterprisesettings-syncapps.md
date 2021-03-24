---
title: syncApps 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05d464c037d882e89054aad111a5185ac91cc631
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141167"
---
# <a name="syncapps-action"></a><span data-ttu-id="2a1c9-103">syncApps 操作</span><span class="sxs-lookup"><span data-stu-id="2a1c9-103">syncApps action</span></span>

<span data-ttu-id="2a1c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a1c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a1c9-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a1c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a1c9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a1c9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a1c9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a1c9-108">Prerequisites</span></span>
<span data-ttu-id="2a1c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a1c9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a1c9-111">Permission type</span></span>|<span data-ttu-id="2a1c9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a1c9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a1c9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a1c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a1c9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a1c9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a1c9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a1c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a1c9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-116">Not supported.</span></span>|
|<span data-ttu-id="2a1c9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a1c9-117">Application</span></span>|<span data-ttu-id="2a1c9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a1c9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a1c9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a1c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

## <a name="request-headers"></a><span data-ttu-id="2a1c9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a1c9-120">Request headers</span></span>
|<span data-ttu-id="2a1c9-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a1c9-121">Header</span></span>|<span data-ttu-id="2a1c9-122">值</span><span class="sxs-lookup"><span data-stu-id="2a1c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a1c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a1c9-123">Authorization</span></span>|<span data-ttu-id="2a1c9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a1c9-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a1c9-125">Accept</span></span>|<span data-ttu-id="2a1c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a1c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a1c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a1c9-127">Request body</span></span>
<span data-ttu-id="2a1c9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a1c9-129">响应</span><span class="sxs-lookup"><span data-stu-id="2a1c9-129">Response</span></span>
<span data-ttu-id="2a1c9-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a1c9-131">示例</span><span class="sxs-lookup"><span data-stu-id="2a1c9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a1c9-132">请求</span><span class="sxs-lookup"><span data-stu-id="2a1c9-132">Request</span></span>
<span data-ttu-id="2a1c9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

### <a name="response"></a><span data-ttu-id="2a1c9-134">响应</span><span class="sxs-lookup"><span data-stu-id="2a1c9-134">Response</span></span>
<span data-ttu-id="2a1c9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a1c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





---
title: uploadDepToken 操作
description: 上传新的设备注册程序令牌
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 949b00571e371b6a6dcbcc82a771ddf32f688132
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696704"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="f5992-103">uploadDepToken 操作</span><span class="sxs-lookup"><span data-stu-id="f5992-103">uploadDepToken action</span></span>

<span data-ttu-id="f5992-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5992-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5992-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5992-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5992-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5992-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5992-107">上传新的设备注册程序令牌</span><span class="sxs-lookup"><span data-stu-id="f5992-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5992-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5992-108">Prerequisites</span></span>
<span data-ttu-id="f5992-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5992-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5992-111">Permission type</span></span>|<span data-ttu-id="f5992-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5992-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5992-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5992-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5992-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5992-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f5992-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5992-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5992-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5992-116">Not supported.</span></span>|
|<span data-ttu-id="f5992-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5992-117">Application</span></span>|<span data-ttu-id="f5992-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5992-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5992-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5992-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="f5992-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5992-120">Request headers</span></span>
|<span data-ttu-id="f5992-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5992-121">Header</span></span>|<span data-ttu-id="f5992-122">值</span><span class="sxs-lookup"><span data-stu-id="f5992-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5992-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5992-123">Authorization</span></span>|<span data-ttu-id="f5992-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5992-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5992-125">接受</span><span class="sxs-lookup"><span data-stu-id="f5992-125">Accept</span></span>|<span data-ttu-id="f5992-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5992-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5992-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5992-127">Request body</span></span>
<span data-ttu-id="f5992-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5992-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f5992-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f5992-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f5992-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5992-130">Property</span></span>|<span data-ttu-id="f5992-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5992-131">Type</span></span>|<span data-ttu-id="f5992-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5992-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5992-133">appleId</span><span class="sxs-lookup"><span data-stu-id="f5992-133">appleId</span></span>|<span data-ttu-id="f5992-134">String</span><span class="sxs-lookup"><span data-stu-id="f5992-134">String</span></span>|<span data-ttu-id="f5992-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5992-135">Not yet documented</span></span>|
|<span data-ttu-id="f5992-136">depToken</span><span class="sxs-lookup"><span data-stu-id="f5992-136">depToken</span></span>|<span data-ttu-id="f5992-137">String</span><span class="sxs-lookup"><span data-stu-id="f5992-137">String</span></span>|<span data-ttu-id="f5992-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5992-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f5992-139">响应</span><span class="sxs-lookup"><span data-stu-id="f5992-139">Response</span></span>
<span data-ttu-id="f5992-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f5992-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5992-141">示例</span><span class="sxs-lookup"><span data-stu-id="f5992-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5992-142">请求</span><span class="sxs-lookup"><span data-stu-id="f5992-142">Request</span></span>
<span data-ttu-id="f5992-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5992-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="f5992-144">响应</span><span class="sxs-lookup"><span data-stu-id="f5992-144">Response</span></span>
<span data-ttu-id="f5992-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5992-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






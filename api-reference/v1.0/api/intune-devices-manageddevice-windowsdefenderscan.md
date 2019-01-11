---
title: windowsDefenderScan 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad9a89fa67c7e6e7b5378bae54b4eb4affbfd852
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891677"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="42515-103">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="42515-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="42515-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="42515-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42515-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42515-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42515-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="42515-106">Prerequisites</span></span>
<span data-ttu-id="42515-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="42515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42515-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42515-109">Permission type</span></span>|<span data-ttu-id="42515-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42515-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42515-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42515-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42515-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="42515-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="42515-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42515-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42515-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="42515-114">Not supported.</span></span>|
|<span data-ttu-id="42515-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="42515-115">Application</span></span>|<span data-ttu-id="42515-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42515-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42515-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42515-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="42515-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="42515-118">Request headers</span></span>
|<span data-ttu-id="42515-119">标头</span><span class="sxs-lookup"><span data-stu-id="42515-119">Header</span></span>|<span data-ttu-id="42515-120">值</span><span class="sxs-lookup"><span data-stu-id="42515-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42515-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42515-121">Authorization</span></span>|<span data-ttu-id="42515-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42515-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42515-123">Accept</span><span class="sxs-lookup"><span data-stu-id="42515-123">Accept</span></span>|<span data-ttu-id="42515-124">application/json</span><span class="sxs-lookup"><span data-stu-id="42515-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42515-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="42515-125">Request body</span></span>
<span data-ttu-id="42515-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42515-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42515-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="42515-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42515-128">属性</span><span class="sxs-lookup"><span data-stu-id="42515-128">Property</span></span>|<span data-ttu-id="42515-129">类型</span><span class="sxs-lookup"><span data-stu-id="42515-129">Type</span></span>|<span data-ttu-id="42515-130">说明</span><span class="sxs-lookup"><span data-stu-id="42515-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42515-131">quickScan</span><span class="sxs-lookup"><span data-stu-id="42515-131">quickScan</span></span>|<span data-ttu-id="42515-132">布尔</span><span class="sxs-lookup"><span data-stu-id="42515-132">Boolean</span></span>|<span data-ttu-id="42515-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42515-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42515-134">响应</span><span class="sxs-lookup"><span data-stu-id="42515-134">Response</span></span>
<span data-ttu-id="42515-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="42515-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42515-136">示例</span><span class="sxs-lookup"><span data-stu-id="42515-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="42515-137">请求</span><span class="sxs-lookup"><span data-stu-id="42515-137">Request</span></span>
<span data-ttu-id="42515-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42515-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="42515-139">响应</span><span class="sxs-lookup"><span data-stu-id="42515-139">Response</span></span>
<span data-ttu-id="42515-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42515-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




---
title: 删除 embeddedSIMDeviceState
description: 删除 embeddedSIMDeviceState。
author: tfitzmac
ms.openlocfilehash: a99ee168896971e4051f93aaea527aa4c24a1f07
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338960"
---
# <a name="delete-embeddedsimdevicestate"></a><span data-ttu-id="a4271-103">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="a4271-103">Delete embeddedSIMDeviceState</span></span>

> <span data-ttu-id="a4271-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4271-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4271-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4271-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4271-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4271-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4271-107">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="a4271-107">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4271-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4271-108">Prerequisites</span></span>
<span data-ttu-id="a4271-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a4271-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4271-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4271-111">Permission type</span></span>|<span data-ttu-id="a4271-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4271-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4271-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4271-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4271-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4271-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4271-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4271-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4271-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4271-116">Not supported.</span></span>|
|<span data-ttu-id="a4271-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4271-117">Application</span></span>|<span data-ttu-id="a4271-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4271-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4271-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4271-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a4271-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4271-120">Request headers</span></span>
|<span data-ttu-id="a4271-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4271-121">Header</span></span>|<span data-ttu-id="a4271-122">值</span><span class="sxs-lookup"><span data-stu-id="a4271-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4271-123">授权</span><span class="sxs-lookup"><span data-stu-id="a4271-123">Authorization</span></span>|<span data-ttu-id="a4271-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4271-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4271-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4271-125">Accept</span></span>|<span data-ttu-id="a4271-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4271-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4271-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4271-127">Request body</span></span>
<span data-ttu-id="a4271-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4271-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4271-129">响应</span><span class="sxs-lookup"><span data-stu-id="a4271-129">Response</span></span>
<span data-ttu-id="a4271-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4271-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4271-131">示例</span><span class="sxs-lookup"><span data-stu-id="a4271-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4271-132">请求</span><span class="sxs-lookup"><span data-stu-id="a4271-132">Request</span></span>
<span data-ttu-id="a4271-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4271-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="a4271-134">响应</span><span class="sxs-lookup"><span data-stu-id="a4271-134">Response</span></span>
<span data-ttu-id="a4271-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4271-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






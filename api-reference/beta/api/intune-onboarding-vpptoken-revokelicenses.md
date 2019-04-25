---
title: revokeLicenses 操作
description: 吊销与特定 appleVolumePurchaseProgramToken 相关联的许可证
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6799edd63f555275ea5f4142844c55611923ac5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527929"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="32314-103">revokeLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="32314-103">revokeLicenses action</span></span>

> <span data-ttu-id="32314-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32314-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32314-106">吊销与特定 appleVolumePurchaseProgramToken 相关联的许可证</span><span class="sxs-lookup"><span data-stu-id="32314-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32314-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="32314-107">Prerequisites</span></span>
<span data-ttu-id="32314-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32314-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32314-110">Permission type</span></span>|<span data-ttu-id="32314-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32314-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32314-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32314-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32314-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32314-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32314-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32314-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32314-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32314-115">Not supported.</span></span>|
|<span data-ttu-id="32314-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32314-116">Application</span></span>|<span data-ttu-id="32314-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="32314-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32314-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32314-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="32314-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="32314-119">Request headers</span></span>
|<span data-ttu-id="32314-120">标头</span><span class="sxs-lookup"><span data-stu-id="32314-120">Header</span></span>|<span data-ttu-id="32314-121">值</span><span class="sxs-lookup"><span data-stu-id="32314-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32314-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32314-122">Authorization</span></span>|<span data-ttu-id="32314-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32314-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32314-124">接受</span><span class="sxs-lookup"><span data-stu-id="32314-124">Accept</span></span>|<span data-ttu-id="32314-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32314-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32314-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32314-126">Request body</span></span>
<span data-ttu-id="32314-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32314-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32314-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="32314-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32314-129">属性</span><span class="sxs-lookup"><span data-stu-id="32314-129">Property</span></span>|<span data-ttu-id="32314-130">类型</span><span class="sxs-lookup"><span data-stu-id="32314-130">Type</span></span>|<span data-ttu-id="32314-131">说明</span><span class="sxs-lookup"><span data-stu-id="32314-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32314-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="32314-132">notifyManagedDevices</span></span>|<span data-ttu-id="32314-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="32314-133">Boolean</span></span>|<span data-ttu-id="32314-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="32314-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32314-135">响应</span><span class="sxs-lookup"><span data-stu-id="32314-135">Response</span></span>
<span data-ttu-id="32314-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32314-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32314-137">示例</span><span class="sxs-lookup"><span data-stu-id="32314-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="32314-138">请求</span><span class="sxs-lookup"><span data-stu-id="32314-138">Request</span></span>
<span data-ttu-id="32314-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32314-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="32314-140">响应</span><span class="sxs-lookup"><span data-stu-id="32314-140">Response</span></span>
<span data-ttu-id="32314-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32314-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






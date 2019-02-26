---
title: uploadDepToken 操作
description: 上传新的设备注册程序令牌
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41381bd722657333d1f4471ac81d2f2dbf884e8d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162158"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="619af-103">uploadDepToken 操作</span><span class="sxs-lookup"><span data-stu-id="619af-103">uploadDepToken action</span></span>

> <span data-ttu-id="619af-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="619af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="619af-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="619af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="619af-106">上传新的设备注册程序令牌</span><span class="sxs-lookup"><span data-stu-id="619af-106">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="619af-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="619af-107">Prerequisites</span></span>
<span data-ttu-id="619af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="619af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="619af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="619af-110">Permission type</span></span>|<span data-ttu-id="619af-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="619af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="619af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="619af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="619af-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="619af-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="619af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="619af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="619af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="619af-115">Not supported.</span></span>|
|<span data-ttu-id="619af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="619af-116">Application</span></span>|<span data-ttu-id="619af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="619af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="619af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="619af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="619af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="619af-119">Request headers</span></span>
|<span data-ttu-id="619af-120">标头</span><span class="sxs-lookup"><span data-stu-id="619af-120">Header</span></span>|<span data-ttu-id="619af-121">值</span><span class="sxs-lookup"><span data-stu-id="619af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="619af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="619af-122">Authorization</span></span>|<span data-ttu-id="619af-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="619af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="619af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="619af-124">Accept</span></span>|<span data-ttu-id="619af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="619af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="619af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="619af-126">Request body</span></span>
<span data-ttu-id="619af-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="619af-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="619af-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="619af-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="619af-129">属性</span><span class="sxs-lookup"><span data-stu-id="619af-129">Property</span></span>|<span data-ttu-id="619af-130">类型</span><span class="sxs-lookup"><span data-stu-id="619af-130">Type</span></span>|<span data-ttu-id="619af-131">说明</span><span class="sxs-lookup"><span data-stu-id="619af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="619af-132">appleId</span><span class="sxs-lookup"><span data-stu-id="619af-132">appleId</span></span>|<span data-ttu-id="619af-133">String</span><span class="sxs-lookup"><span data-stu-id="619af-133">String</span></span>|<span data-ttu-id="619af-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="619af-134">Not yet documented</span></span>|
|<span data-ttu-id="619af-135">depToken</span><span class="sxs-lookup"><span data-stu-id="619af-135">depToken</span></span>|<span data-ttu-id="619af-136">String</span><span class="sxs-lookup"><span data-stu-id="619af-136">String</span></span>|<span data-ttu-id="619af-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="619af-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="619af-138">响应</span><span class="sxs-lookup"><span data-stu-id="619af-138">Response</span></span>
<span data-ttu-id="619af-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="619af-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="619af-140">示例</span><span class="sxs-lookup"><span data-stu-id="619af-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="619af-141">请求</span><span class="sxs-lookup"><span data-stu-id="619af-141">Request</span></span>
<span data-ttu-id="619af-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="619af-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="619af-143">响应</span><span class="sxs-lookup"><span data-stu-id="619af-143">Response</span></span>
<span data-ttu-id="619af-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="619af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





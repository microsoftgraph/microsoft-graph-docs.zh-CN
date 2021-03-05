---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1be868185e634ba74f9f58f1ab4c388efcf5ed3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474867"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="298ba-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="298ba-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="298ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="298ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="298ba-105">**重要提示：** Microsoft Graph 中 /beta 版本的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="298ba-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="298ba-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="298ba-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="298ba-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="298ba-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="298ba-108">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="298ba-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="298ba-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="298ba-109">Prerequisites</span></span>
<span data-ttu-id="298ba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="298ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="298ba-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="298ba-112">Permission type</span></span>|<span data-ttu-id="298ba-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="298ba-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="298ba-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="298ba-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="298ba-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="298ba-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="298ba-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="298ba-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="298ba-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="298ba-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="298ba-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="298ba-118">Not supported.</span></span>|
|<span data-ttu-id="298ba-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="298ba-119">Application</span></span>||
| <span data-ttu-id="298ba-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="298ba-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="298ba-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="298ba-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="298ba-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="298ba-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="298ba-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="298ba-123">Request headers</span></span>
|<span data-ttu-id="298ba-124">标头</span><span class="sxs-lookup"><span data-stu-id="298ba-124">Header</span></span>|<span data-ttu-id="298ba-125">值</span><span class="sxs-lookup"><span data-stu-id="298ba-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="298ba-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="298ba-126">Authorization</span></span>|<span data-ttu-id="298ba-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="298ba-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="298ba-128">接受</span><span class="sxs-lookup"><span data-stu-id="298ba-128">Accept</span></span>|<span data-ttu-id="298ba-129">application/json</span><span class="sxs-lookup"><span data-stu-id="298ba-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="298ba-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="298ba-130">Request body</span></span>
<span data-ttu-id="298ba-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="298ba-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="298ba-132">响应</span><span class="sxs-lookup"><span data-stu-id="298ba-132">Response</span></span>
<span data-ttu-id="298ba-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="298ba-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="298ba-134">示例</span><span class="sxs-lookup"><span data-stu-id="298ba-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="298ba-135">请求</span><span class="sxs-lookup"><span data-stu-id="298ba-135">Request</span></span>
<span data-ttu-id="298ba-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="298ba-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="298ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="298ba-137">Response</span></span>
<span data-ttu-id="298ba-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="298ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











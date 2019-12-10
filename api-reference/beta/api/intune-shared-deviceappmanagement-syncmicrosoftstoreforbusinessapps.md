---
title: syncMicrosoftStoreForBusinessApps 操作
description: 将 Intune 帐户与适用于企业的 Microsoft Store 同步
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff9774f602b182ad18791004c71404dc3e298027
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940178"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="148f4-103">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="148f4-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="148f4-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="148f4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="148f4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="148f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="148f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="148f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148f4-107">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="148f4-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="148f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="148f4-108">Prerequisites</span></span>
<span data-ttu-id="148f4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="148f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="148f4-111">Permission type</span></span>|<span data-ttu-id="148f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="148f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="148f4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="148f4-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="148f4-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="148f4-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148f4-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="148f4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="148f4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="148f4-117">Not supported.</span></span>|
|<span data-ttu-id="148f4-118">Application</span><span class="sxs-lookup"><span data-stu-id="148f4-118">Application</span></span>||
| <span data-ttu-id="148f4-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="148f4-119">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="148f4-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148f4-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="148f4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="148f4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="148f4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="148f4-122">Request headers</span></span>
|<span data-ttu-id="148f4-123">标头</span><span class="sxs-lookup"><span data-stu-id="148f4-123">Header</span></span>|<span data-ttu-id="148f4-124">值</span><span class="sxs-lookup"><span data-stu-id="148f4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148f4-125">授权</span><span class="sxs-lookup"><span data-stu-id="148f4-125">Authorization</span></span>|<span data-ttu-id="148f4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="148f4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148f4-127">接受</span><span class="sxs-lookup"><span data-stu-id="148f4-127">Accept</span></span>|<span data-ttu-id="148f4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="148f4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148f4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="148f4-129">Request body</span></span>
<span data-ttu-id="148f4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="148f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="148f4-131">响应</span><span class="sxs-lookup"><span data-stu-id="148f4-131">Response</span></span>
<span data-ttu-id="148f4-132">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="148f4-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="148f4-133">示例</span><span class="sxs-lookup"><span data-stu-id="148f4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="148f4-134">请求</span><span class="sxs-lookup"><span data-stu-id="148f4-134">Request</span></span>
<span data-ttu-id="148f4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="148f4-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="148f4-136">响应</span><span class="sxs-lookup"><span data-stu-id="148f4-136">Response</span></span>
<span data-ttu-id="148f4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="148f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












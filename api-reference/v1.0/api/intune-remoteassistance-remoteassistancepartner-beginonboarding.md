---
title: beginOnboarding 操作
description: 尚未记录
ms.openlocfilehash: a410558bccd5c0d76e9515e14dd161bfc9a3b3d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009974"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="f388d-103">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="f388d-103">beginOnboarding action</span></span>

> <span data-ttu-id="f388d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f388d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f388d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f388d-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f388d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f388d-106">Prerequisites</span></span>
<span data-ttu-id="f388d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f388d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f388d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f388d-109">Permission type</span></span>|<span data-ttu-id="f388d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f388d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f388d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f388d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f388d-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f388d-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f388d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f388d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f388d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f388d-114">Not supported.</span></span>|
|<span data-ttu-id="f388d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f388d-115">Application</span></span>|<span data-ttu-id="f388d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f388d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f388d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f388d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="f388d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f388d-118">Request headers</span></span>
|<span data-ttu-id="f388d-119">标头</span><span class="sxs-lookup"><span data-stu-id="f388d-119">Header</span></span>|<span data-ttu-id="f388d-120">值</span><span class="sxs-lookup"><span data-stu-id="f388d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f388d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f388d-121">Authorization</span></span>|<span data-ttu-id="f388d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f388d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f388d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f388d-123">Accept</span></span>|<span data-ttu-id="f388d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f388d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f388d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f388d-125">Request body</span></span>
<span data-ttu-id="f388d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f388d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f388d-127">响应</span><span class="sxs-lookup"><span data-stu-id="f388d-127">Response</span></span>
<span data-ttu-id="f388d-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f388d-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f388d-129">示例</span><span class="sxs-lookup"><span data-stu-id="f388d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f388d-130">请求</span><span class="sxs-lookup"><span data-stu-id="f388d-130">Request</span></span>
<span data-ttu-id="f388d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f388d-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="f388d-132">响应</span><span class="sxs-lookup"><span data-stu-id="f388d-132">Response</span></span>
<span data-ttu-id="f388d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f388d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




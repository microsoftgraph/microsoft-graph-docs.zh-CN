---
title: 删除 webApp
description: 删除 webApp。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 726b5e1824a4d8b8a26a20d5975a757d5474ad52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855396"
---
# <a name="delete-webapp"></a><span data-ttu-id="ee078-103">删除 webApp</span><span class="sxs-lookup"><span data-stu-id="ee078-103">Delete webApp</span></span>

> <span data-ttu-id="ee078-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ee078-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee078-105">删除 [webApp](../resources/intune-apps-webapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ee078-105">Deletes a [webApp](../resources/intune-apps-webapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee078-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ee078-106">Prerequisites</span></span>
<span data-ttu-id="ee078-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ee078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee078-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee078-109">Permission type</span></span>|<span data-ttu-id="ee078-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ee078-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee078-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee078-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee078-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee078-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee078-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee078-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee078-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee078-114">Not supported.</span></span>|
|<span data-ttu-id="ee078-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee078-115">Application</span></span>|<span data-ttu-id="ee078-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee078-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee078-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee078-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ee078-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee078-118">Request headers</span></span>
|<span data-ttu-id="ee078-119">标头</span><span class="sxs-lookup"><span data-stu-id="ee078-119">Header</span></span>|<span data-ttu-id="ee078-120">值</span><span class="sxs-lookup"><span data-stu-id="ee078-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee078-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee078-121">Authorization</span></span>|<span data-ttu-id="ee078-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ee078-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee078-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ee078-123">Accept</span></span>|<span data-ttu-id="ee078-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ee078-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee078-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee078-125">Request body</span></span>
<span data-ttu-id="ee078-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee078-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee078-127">响应</span><span class="sxs-lookup"><span data-stu-id="ee078-127">Response</span></span>
<span data-ttu-id="ee078-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ee078-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee078-129">示例</span><span class="sxs-lookup"><span data-stu-id="ee078-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee078-130">请求</span><span class="sxs-lookup"><span data-stu-id="ee078-130">Request</span></span>
<span data-ttu-id="ee078-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee078-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ee078-132">响应</span><span class="sxs-lookup"><span data-stu-id="ee078-132">Response</span></span>
<span data-ttu-id="ee078-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




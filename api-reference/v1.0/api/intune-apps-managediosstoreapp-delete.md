---
title: 删除 managedIOSStoreApp
description: 删除 managedIOSStoreApp
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c39ca3ce13f4d631d204f391456d72701bce14c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830721"
---
# <a name="delete-managediosstoreapp"></a><span data-ttu-id="56b7c-103">删除 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="56b7c-103">Delete managedIOSStoreApp</span></span>

> <span data-ttu-id="56b7c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="56b7c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56b7c-105">删除 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="56b7c-105">Deletes a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56b7c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="56b7c-106">Prerequisites</span></span>
<span data-ttu-id="56b7c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="56b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56b7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56b7c-109">Permission type</span></span>|<span data-ttu-id="56b7c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56b7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56b7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56b7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56b7c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56b7c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56b7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56b7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56b7c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56b7c-114">Not supported.</span></span>|
|<span data-ttu-id="56b7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56b7c-115">Application</span></span>|<span data-ttu-id="56b7c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56b7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56b7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56b7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="56b7c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="56b7c-118">Request headers</span></span>
|<span data-ttu-id="56b7c-119">标头</span><span class="sxs-lookup"><span data-stu-id="56b7c-119">Header</span></span>|<span data-ttu-id="56b7c-120">值</span><span class="sxs-lookup"><span data-stu-id="56b7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56b7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56b7c-121">Authorization</span></span>|<span data-ttu-id="56b7c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56b7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56b7c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="56b7c-123">Accept</span></span>|<span data-ttu-id="56b7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56b7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56b7c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="56b7c-125">Request body</span></span>
<span data-ttu-id="56b7c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56b7c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56b7c-127">响应</span><span class="sxs-lookup"><span data-stu-id="56b7c-127">Response</span></span>
<span data-ttu-id="56b7c-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="56b7c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56b7c-129">示例</span><span class="sxs-lookup"><span data-stu-id="56b7c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="56b7c-130">请求</span><span class="sxs-lookup"><span data-stu-id="56b7c-130">Request</span></span>
<span data-ttu-id="56b7c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56b7c-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="56b7c-132">响应</span><span class="sxs-lookup"><span data-stu-id="56b7c-132">Response</span></span>
<span data-ttu-id="56b7c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56b7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




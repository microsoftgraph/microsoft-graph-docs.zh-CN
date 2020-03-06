---
title: downloadApplePushNotificationCertificateSigningRequest 函数
description: 下载 Apple 推送通知证书签名请求
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e9d95c9db9bfa580ede350c3e6c1500192c545a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513656"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="88754-103">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="88754-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

<span data-ttu-id="88754-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88754-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88754-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88754-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88754-106">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="88754-106">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88754-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="88754-107">Prerequisites</span></span>
<span data-ttu-id="88754-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88754-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="88754-110">Permission type</span></span>|<span data-ttu-id="88754-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88754-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88754-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88754-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88754-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88754-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88754-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88754-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88754-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88754-115">Not supported.</span></span>|
|<span data-ttu-id="88754-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="88754-116">Application</span></span>|<span data-ttu-id="88754-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="88754-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88754-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88754-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="88754-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="88754-119">Request headers</span></span>
|<span data-ttu-id="88754-120">标头</span><span class="sxs-lookup"><span data-stu-id="88754-120">Header</span></span>|<span data-ttu-id="88754-121">值</span><span class="sxs-lookup"><span data-stu-id="88754-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88754-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="88754-122">Authorization</span></span>|<span data-ttu-id="88754-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88754-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88754-124">接受</span><span class="sxs-lookup"><span data-stu-id="88754-124">Accept</span></span>|<span data-ttu-id="88754-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88754-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88754-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88754-126">Request body</span></span>
<span data-ttu-id="88754-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88754-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88754-128">响应</span><span class="sxs-lookup"><span data-stu-id="88754-128">Response</span></span>
<span data-ttu-id="88754-129">如果成功，此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="88754-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88754-130">示例</span><span class="sxs-lookup"><span data-stu-id="88754-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88754-131">请求</span><span class="sxs-lookup"><span data-stu-id="88754-131">Request</span></span>
<span data-ttu-id="88754-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88754-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="88754-133">响应</span><span class="sxs-lookup"><span data-stu-id="88754-133">Response</span></span>
<span data-ttu-id="88754-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88754-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```





---
title: downloadApplePushNotificationCertificateSigningRequest 函数
description: 下载 Apple 推送通知证书签名请求
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c532c55386a25b23ca3cdc218a936b9f8e84adf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997006"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="d0990-103">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="d0990-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="d0990-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0990-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0990-105">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="d0990-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0990-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0990-106">Prerequisites</span></span>
<span data-ttu-id="d0990-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0990-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0990-109">Permission type</span></span>|<span data-ttu-id="d0990-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0990-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0990-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0990-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0990-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0990-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0990-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0990-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0990-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0990-114">Not supported.</span></span>|
|<span data-ttu-id="d0990-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0990-115">Application</span></span>|<span data-ttu-id="d0990-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0990-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0990-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0990-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="d0990-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0990-118">Request headers</span></span>
|<span data-ttu-id="d0990-119">标头</span><span class="sxs-lookup"><span data-stu-id="d0990-119">Header</span></span>|<span data-ttu-id="d0990-120">值</span><span class="sxs-lookup"><span data-stu-id="d0990-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0990-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0990-121">Authorization</span></span>|<span data-ttu-id="d0990-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0990-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0990-123">接受</span><span class="sxs-lookup"><span data-stu-id="d0990-123">Accept</span></span>|<span data-ttu-id="d0990-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0990-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0990-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0990-125">Request body</span></span>
<span data-ttu-id="d0990-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0990-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0990-127">响应</span><span class="sxs-lookup"><span data-stu-id="d0990-127">Response</span></span>
<span data-ttu-id="d0990-128">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="d0990-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0990-129">示例</span><span class="sxs-lookup"><span data-stu-id="d0990-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0990-130">请求</span><span class="sxs-lookup"><span data-stu-id="d0990-130">Request</span></span>
<span data-ttu-id="d0990-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0990-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="d0990-132">响应</span><span class="sxs-lookup"><span data-stu-id="d0990-132">Response</span></span>
<span data-ttu-id="d0990-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0990-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




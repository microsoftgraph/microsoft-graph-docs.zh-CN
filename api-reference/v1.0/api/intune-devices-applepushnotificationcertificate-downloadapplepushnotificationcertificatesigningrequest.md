---
title: downloadApplePushNotificationCertificateSigningRequest 函数
description: 下载 Apple 推送通知证书签名请求
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09bbadd2e0874bdc461f965ff12544716e4de9d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583492"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="90bdc-103">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="90bdc-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="90bdc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90bdc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90bdc-105">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="90bdc-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90bdc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="90bdc-106">Prerequisites</span></span>
<span data-ttu-id="90bdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90bdc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90bdc-109">Permission type</span></span>|<span data-ttu-id="90bdc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90bdc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90bdc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90bdc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90bdc-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90bdc-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90bdc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90bdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90bdc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90bdc-114">Not supported.</span></span>|
|<span data-ttu-id="90bdc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90bdc-115">Application</span></span>|<span data-ttu-id="90bdc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90bdc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90bdc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90bdc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="90bdc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90bdc-118">Request headers</span></span>
|<span data-ttu-id="90bdc-119">标头</span><span class="sxs-lookup"><span data-stu-id="90bdc-119">Header</span></span>|<span data-ttu-id="90bdc-120">值</span><span class="sxs-lookup"><span data-stu-id="90bdc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90bdc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90bdc-121">Authorization</span></span>|<span data-ttu-id="90bdc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90bdc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90bdc-123">接受</span><span class="sxs-lookup"><span data-stu-id="90bdc-123">Accept</span></span>|<span data-ttu-id="90bdc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90bdc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90bdc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="90bdc-125">Request body</span></span>
<span data-ttu-id="90bdc-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90bdc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90bdc-127">响应</span><span class="sxs-lookup"><span data-stu-id="90bdc-127">Response</span></span>
<span data-ttu-id="90bdc-128">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="90bdc-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90bdc-129">示例</span><span class="sxs-lookup"><span data-stu-id="90bdc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="90bdc-130">请求</span><span class="sxs-lookup"><span data-stu-id="90bdc-130">Request</span></span>
<span data-ttu-id="90bdc-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90bdc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="90bdc-132">响应</span><span class="sxs-lookup"><span data-stu-id="90bdc-132">Response</span></span>
<span data-ttu-id="90bdc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90bdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




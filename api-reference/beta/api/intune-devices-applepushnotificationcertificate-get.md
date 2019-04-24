---
title: 获取 applePushNotificationCertificate
description: 读取 applePushNotificationCertificate 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d68ef5d169eb37c3a7b0c3561a612df8b670086
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466194"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="639ab-103">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="639ab-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="639ab-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="639ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="639ab-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="639ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="639ab-106">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="639ab-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="639ab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="639ab-107">Prerequisites</span></span>
<span data-ttu-id="639ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="639ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="639ab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="639ab-110">Permission type</span></span>|<span data-ttu-id="639ab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="639ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="639ab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="639ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="639ab-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="639ab-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="639ab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="639ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="639ab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="639ab-115">Not supported.</span></span>|
|<span data-ttu-id="639ab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="639ab-116">Application</span></span>|<span data-ttu-id="639ab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="639ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="639ab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="639ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="639ab-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="639ab-119">Optional query parameters</span></span>
<span data-ttu-id="639ab-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="639ab-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="639ab-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="639ab-121">Request headers</span></span>
|<span data-ttu-id="639ab-122">标头</span><span class="sxs-lookup"><span data-stu-id="639ab-122">Header</span></span>|<span data-ttu-id="639ab-123">值</span><span class="sxs-lookup"><span data-stu-id="639ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="639ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="639ab-124">Authorization</span></span>|<span data-ttu-id="639ab-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="639ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="639ab-126">接受</span><span class="sxs-lookup"><span data-stu-id="639ab-126">Accept</span></span>|<span data-ttu-id="639ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="639ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="639ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="639ab-128">Request body</span></span>
<span data-ttu-id="639ab-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="639ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="639ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="639ab-130">Response</span></span>
<span data-ttu-id="639ab-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="639ab-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="639ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="639ab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="639ab-133">请求</span><span class="sxs-lookup"><span data-stu-id="639ab-133">Request</span></span>
<span data-ttu-id="639ab-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="639ab-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="639ab-135">响应</span><span class="sxs-lookup"><span data-stu-id="639ab-135">Response</span></span>
<span data-ttu-id="639ab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="639ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateUploadStatus": "Certificate Upload Status value",
    "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
    "certificate": "Certificate value"
  }
}
```






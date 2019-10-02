---
title: 获取 applePushNotificationCertificate
description: 读取 applePushNotificationCertificate 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e133dbd6d05ee9412f5eee82d7025525ae9d9d52
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364611"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="efb0e-103">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="efb0e-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="efb0e-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efb0e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb0e-105">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efb0e-105">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb0e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="efb0e-106">Prerequisites</span></span>
<span data-ttu-id="efb0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="efb0e-109">Permission type</span></span>|<span data-ttu-id="efb0e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efb0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efb0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efb0e-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="efb0e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="efb0e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efb0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb0e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="efb0e-114">Not supported.</span></span>|
|<span data-ttu-id="efb0e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="efb0e-115">Application</span></span>|<span data-ttu-id="efb0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="efb0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb0e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efb0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efb0e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="efb0e-118">Optional query parameters</span></span>
<span data-ttu-id="efb0e-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="efb0e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efb0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="efb0e-120">Request headers</span></span>
|<span data-ttu-id="efb0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="efb0e-121">Header</span></span>|<span data-ttu-id="efb0e-122">值</span><span class="sxs-lookup"><span data-stu-id="efb0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb0e-123">Authorization</span></span>|<span data-ttu-id="efb0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efb0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="efb0e-125">Accept</span></span>|<span data-ttu-id="efb0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efb0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="efb0e-127">Request body</span></span>
<span data-ttu-id="efb0e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efb0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb0e-129">响应</span><span class="sxs-lookup"><span data-stu-id="efb0e-129">Response</span></span>
<span data-ttu-id="efb0e-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efb0e-130">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="efb0e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb0e-132">请求</span><span class="sxs-lookup"><span data-stu-id="efb0e-132">Request</span></span>
<span data-ttu-id="efb0e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efb0e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="efb0e-134">响应</span><span class="sxs-lookup"><span data-stu-id="efb0e-134">Response</span></span>
<span data-ttu-id="efb0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efb0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Certificate value"
  }
}
```





---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b0726ba347e9dd2c74e2c35c16f60935ac39465
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884887"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="1e375-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1e375-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="1e375-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e375-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e375-105">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e375-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e375-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e375-106">Prerequisites</span></span>
<span data-ttu-id="1e375-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1e375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e375-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e375-109">Permission type</span></span>|<span data-ttu-id="1e375-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e375-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e375-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e375-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e375-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e375-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1e375-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e375-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e375-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e375-114">Not supported.</span></span>|
|<span data-ttu-id="1e375-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e375-115">Application</span></span>|<span data-ttu-id="1e375-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e375-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e375-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e375-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="1e375-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e375-118">Request headers</span></span>
|<span data-ttu-id="1e375-119">标头</span><span class="sxs-lookup"><span data-stu-id="1e375-119">Header</span></span>|<span data-ttu-id="1e375-120">值</span><span class="sxs-lookup"><span data-stu-id="1e375-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e375-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e375-121">Authorization</span></span>|<span data-ttu-id="1e375-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e375-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e375-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1e375-123">Accept</span></span>|<span data-ttu-id="1e375-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e375-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e375-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e375-125">Request body</span></span>
<span data-ttu-id="1e375-126">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e375-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="1e375-127">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e375-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="1e375-128">属性</span><span class="sxs-lookup"><span data-stu-id="1e375-128">Property</span></span>|<span data-ttu-id="1e375-129">类型</span><span class="sxs-lookup"><span data-stu-id="1e375-129">Type</span></span>|<span data-ttu-id="1e375-130">说明</span><span class="sxs-lookup"><span data-stu-id="1e375-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e375-131">id</span><span class="sxs-lookup"><span data-stu-id="1e375-131">id</span></span>|<span data-ttu-id="1e375-132">String</span><span class="sxs-lookup"><span data-stu-id="1e375-132">String</span></span>|<span data-ttu-id="1e375-133">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1e375-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="1e375-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e375-134">appleIdentifier</span></span>|<span data-ttu-id="1e375-135">String</span><span class="sxs-lookup"><span data-stu-id="1e375-135">String</span></span>|<span data-ttu-id="1e375-136">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="1e375-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="1e375-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e375-137">topicIdentifier</span></span>|<span data-ttu-id="1e375-138">String</span><span class="sxs-lookup"><span data-stu-id="1e375-138">String</span></span>|<span data-ttu-id="1e375-139">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="1e375-139">Topic Id.</span></span>|
|<span data-ttu-id="1e375-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e375-140">lastModifiedDateTime</span></span>|<span data-ttu-id="1e375-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e375-141">DateTimeOffset</span></span>|<span data-ttu-id="1e375-142">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1e375-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1e375-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e375-143">expirationDateTime</span></span>|<span data-ttu-id="1e375-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e375-144">DateTimeOffset</span></span>|<span data-ttu-id="1e375-145">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1e375-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1e375-146">certificate</span><span class="sxs-lookup"><span data-stu-id="1e375-146">certificate</span></span>|<span data-ttu-id="1e375-147">String</span><span class="sxs-lookup"><span data-stu-id="1e375-147">String</span></span>|<span data-ttu-id="1e375-148">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1e375-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1e375-149">响应</span><span class="sxs-lookup"><span data-stu-id="1e375-149">Response</span></span>
<span data-ttu-id="1e375-150">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e375-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e375-151">示例</span><span class="sxs-lookup"><span data-stu-id="1e375-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e375-152">请求</span><span class="sxs-lookup"><span data-stu-id="1e375-152">Request</span></span>
<span data-ttu-id="1e375-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e375-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="1e375-154">响应</span><span class="sxs-lookup"><span data-stu-id="1e375-154">Response</span></span>
<span data-ttu-id="1e375-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```




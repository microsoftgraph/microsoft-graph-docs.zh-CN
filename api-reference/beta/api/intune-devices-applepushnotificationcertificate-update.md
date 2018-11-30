---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
ms.openlocfilehash: 7fbb7db93290fb6f455bdcca3053c6f3affb1375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043765"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="b58b3-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b58b3-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="b58b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b58b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b58b3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b58b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b58b3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b58b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b58b3-107">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b58b3-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b58b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b58b3-108">Prerequisites</span></span>
<span data-ttu-id="b58b3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b58b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b58b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b58b3-111">Permission type</span></span>|<span data-ttu-id="b58b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b58b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b58b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b58b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b58b3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b58b3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b58b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b58b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b58b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b58b3-116">Not supported.</span></span>|
|<span data-ttu-id="b58b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b58b3-117">Application</span></span>|<span data-ttu-id="b58b3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b58b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b58b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b58b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b58b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b58b3-120">Request headers</span></span>
|<span data-ttu-id="b58b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="b58b3-121">Header</span></span>|<span data-ttu-id="b58b3-122">值</span><span class="sxs-lookup"><span data-stu-id="b58b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b58b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b58b3-123">Authorization</span></span>|<span data-ttu-id="b58b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b58b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b58b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b58b3-125">Accept</span></span>|<span data-ttu-id="b58b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b58b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b58b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b58b3-127">Request body</span></span>
<span data-ttu-id="b58b3-128">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b58b3-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="b58b3-129">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b58b3-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="b58b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="b58b3-130">Property</span></span>|<span data-ttu-id="b58b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="b58b3-131">Type</span></span>|<span data-ttu-id="b58b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="b58b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b58b3-133">id</span><span class="sxs-lookup"><span data-stu-id="b58b3-133">id</span></span>|<span data-ttu-id="b58b3-134">String</span><span class="sxs-lookup"><span data-stu-id="b58b3-134">String</span></span>|<span data-ttu-id="b58b3-135">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b58b3-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b58b3-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b58b3-136">appleIdentifier</span></span>|<span data-ttu-id="b58b3-137">String</span><span class="sxs-lookup"><span data-stu-id="b58b3-137">String</span></span>|<span data-ttu-id="b58b3-138">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b58b3-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b58b3-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b58b3-139">topicIdentifier</span></span>|<span data-ttu-id="b58b3-140">String</span><span class="sxs-lookup"><span data-stu-id="b58b3-140">String</span></span>|<span data-ttu-id="b58b3-141">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="b58b3-141">Topic Id.</span></span>|
|<span data-ttu-id="b58b3-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b58b3-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b58b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b58b3-143">DateTimeOffset</span></span>|<span data-ttu-id="b58b3-144">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b58b3-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b58b3-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b58b3-145">expirationDateTime</span></span>|<span data-ttu-id="b58b3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b58b3-146">DateTimeOffset</span></span>|<span data-ttu-id="b58b3-147">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b58b3-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b58b3-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b58b3-148">certificateUploadStatus</span></span>|<span data-ttu-id="b58b3-149">字符串</span><span class="sxs-lookup"><span data-stu-id="b58b3-149">String</span></span>|<span data-ttu-id="b58b3-150">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="b58b3-150">The certificate upload status.</span></span>|
|<span data-ttu-id="b58b3-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="b58b3-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="b58b3-152">字符串</span><span class="sxs-lookup"><span data-stu-id="b58b3-152">String</span></span>|<span data-ttu-id="b58b3-153">原因证书上载失败。</span><span class="sxs-lookup"><span data-stu-id="b58b3-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="b58b3-154">certificate</span><span class="sxs-lookup"><span data-stu-id="b58b3-154">certificate</span></span>|<span data-ttu-id="b58b3-155">String</span><span class="sxs-lookup"><span data-stu-id="b58b3-155">String</span></span>|<span data-ttu-id="b58b3-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b58b3-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b58b3-157">响应</span><span class="sxs-lookup"><span data-stu-id="b58b3-157">Response</span></span>
<span data-ttu-id="b58b3-158">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b58b3-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b58b3-159">示例</span><span class="sxs-lookup"><span data-stu-id="b58b3-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="b58b3-160">请求</span><span class="sxs-lookup"><span data-stu-id="b58b3-160">Request</span></span>
<span data-ttu-id="b58b3-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b58b3-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 409

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="b58b3-162">响应</span><span class="sxs-lookup"><span data-stu-id="b58b3-162">Response</span></span>
<span data-ttu-id="b58b3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b58b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
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
```






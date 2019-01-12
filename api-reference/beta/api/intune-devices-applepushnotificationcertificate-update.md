---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6cc1b113b964dbc2f2ffdaae1e52639ec2463f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964835"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="7b01b-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7b01b-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="7b01b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b01b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b01b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b01b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b01b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b01b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b01b-107">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b01b-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b01b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b01b-108">Prerequisites</span></span>
<span data-ttu-id="7b01b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7b01b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b01b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b01b-111">Permission type</span></span>|<span data-ttu-id="7b01b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b01b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b01b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b01b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b01b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b01b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b01b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b01b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b01b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b01b-116">Not supported.</span></span>|
|<span data-ttu-id="7b01b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b01b-117">Application</span></span>|<span data-ttu-id="7b01b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b01b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b01b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b01b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="7b01b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b01b-120">Request headers</span></span>
|<span data-ttu-id="7b01b-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b01b-121">Header</span></span>|<span data-ttu-id="7b01b-122">值</span><span class="sxs-lookup"><span data-stu-id="7b01b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b01b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b01b-123">Authorization</span></span>|<span data-ttu-id="7b01b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b01b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b01b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b01b-125">Accept</span></span>|<span data-ttu-id="7b01b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b01b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b01b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b01b-127">Request body</span></span>
<span data-ttu-id="7b01b-128">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b01b-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="7b01b-129">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b01b-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="7b01b-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b01b-130">Property</span></span>|<span data-ttu-id="7b01b-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b01b-131">Type</span></span>|<span data-ttu-id="7b01b-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b01b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b01b-133">id</span><span class="sxs-lookup"><span data-stu-id="7b01b-133">id</span></span>|<span data-ttu-id="7b01b-134">String</span><span class="sxs-lookup"><span data-stu-id="7b01b-134">String</span></span>|<span data-ttu-id="7b01b-135">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7b01b-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="7b01b-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b01b-136">appleIdentifier</span></span>|<span data-ttu-id="7b01b-137">String</span><span class="sxs-lookup"><span data-stu-id="7b01b-137">String</span></span>|<span data-ttu-id="7b01b-138">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="7b01b-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="7b01b-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b01b-139">topicIdentifier</span></span>|<span data-ttu-id="7b01b-140">String</span><span class="sxs-lookup"><span data-stu-id="7b01b-140">String</span></span>|<span data-ttu-id="7b01b-141">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="7b01b-141">Topic Id.</span></span>|
|<span data-ttu-id="7b01b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b01b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7b01b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b01b-143">DateTimeOffset</span></span>|<span data-ttu-id="7b01b-144">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7b01b-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7b01b-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7b01b-145">expirationDateTime</span></span>|<span data-ttu-id="7b01b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b01b-146">DateTimeOffset</span></span>|<span data-ttu-id="7b01b-147">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7b01b-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7b01b-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="7b01b-148">certificateUploadStatus</span></span>|<span data-ttu-id="7b01b-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7b01b-149">String</span></span>|<span data-ttu-id="7b01b-150">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="7b01b-150">The certificate upload status.</span></span>|
|<span data-ttu-id="7b01b-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="7b01b-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="7b01b-152">字符串</span><span class="sxs-lookup"><span data-stu-id="7b01b-152">String</span></span>|<span data-ttu-id="7b01b-153">原因证书上载失败。</span><span class="sxs-lookup"><span data-stu-id="7b01b-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="7b01b-154">certificate</span><span class="sxs-lookup"><span data-stu-id="7b01b-154">certificate</span></span>|<span data-ttu-id="7b01b-155">String</span><span class="sxs-lookup"><span data-stu-id="7b01b-155">String</span></span>|<span data-ttu-id="7b01b-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7b01b-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7b01b-157">响应</span><span class="sxs-lookup"><span data-stu-id="7b01b-157">Response</span></span>
<span data-ttu-id="7b01b-158">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b01b-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b01b-159">示例</span><span class="sxs-lookup"><span data-stu-id="7b01b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b01b-160">请求</span><span class="sxs-lookup"><span data-stu-id="7b01b-160">Request</span></span>
<span data-ttu-id="7b01b-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b01b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b01b-162">响应</span><span class="sxs-lookup"><span data-stu-id="7b01b-162">Response</span></span>
<span data-ttu-id="7b01b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b01b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






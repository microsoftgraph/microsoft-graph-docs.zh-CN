---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e14e4056f0428548e0b910c8647dc4442efe4abd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397482"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="58a71-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="58a71-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="58a71-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="58a71-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58a71-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58a71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58a71-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58a71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a71-107">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58a71-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a71-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="58a71-108">Prerequisites</span></span>
<span data-ttu-id="58a71-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="58a71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58a71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58a71-111">Permission type</span></span>|<span data-ttu-id="58a71-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58a71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58a71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58a71-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a71-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58a71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58a71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58a71-116">Not supported.</span></span>|
|<span data-ttu-id="58a71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="58a71-117">Application</span></span>|<span data-ttu-id="58a71-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="58a71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58a71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="58a71-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58a71-120">Request headers</span></span>
|<span data-ttu-id="58a71-121">标头</span><span class="sxs-lookup"><span data-stu-id="58a71-121">Header</span></span>|<span data-ttu-id="58a71-122">值</span><span class="sxs-lookup"><span data-stu-id="58a71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a71-123">Authorization</span></span>|<span data-ttu-id="58a71-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58a71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58a71-125">Accept</span></span>|<span data-ttu-id="58a71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58a71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58a71-127">Request body</span></span>
<span data-ttu-id="58a71-128">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58a71-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="58a71-129">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58a71-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="58a71-130">属性</span><span class="sxs-lookup"><span data-stu-id="58a71-130">Property</span></span>|<span data-ttu-id="58a71-131">类型</span><span class="sxs-lookup"><span data-stu-id="58a71-131">Type</span></span>|<span data-ttu-id="58a71-132">说明</span><span class="sxs-lookup"><span data-stu-id="58a71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a71-133">id</span><span class="sxs-lookup"><span data-stu-id="58a71-133">id</span></span>|<span data-ttu-id="58a71-134">String</span><span class="sxs-lookup"><span data-stu-id="58a71-134">String</span></span>|<span data-ttu-id="58a71-135">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="58a71-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="58a71-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="58a71-136">appleIdentifier</span></span>|<span data-ttu-id="58a71-137">String</span><span class="sxs-lookup"><span data-stu-id="58a71-137">String</span></span>|<span data-ttu-id="58a71-138">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="58a71-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="58a71-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="58a71-139">topicIdentifier</span></span>|<span data-ttu-id="58a71-140">String</span><span class="sxs-lookup"><span data-stu-id="58a71-140">String</span></span>|<span data-ttu-id="58a71-141">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="58a71-141">Topic Id.</span></span>|
|<span data-ttu-id="58a71-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58a71-142">lastModifiedDateTime</span></span>|<span data-ttu-id="58a71-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a71-143">DateTimeOffset</span></span>|<span data-ttu-id="58a71-144">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58a71-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="58a71-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58a71-145">expirationDateTime</span></span>|<span data-ttu-id="58a71-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a71-146">DateTimeOffset</span></span>|<span data-ttu-id="58a71-147">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58a71-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="58a71-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="58a71-148">certificateUploadStatus</span></span>|<span data-ttu-id="58a71-149">String</span><span class="sxs-lookup"><span data-stu-id="58a71-149">String</span></span>|<span data-ttu-id="58a71-150">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="58a71-150">The certificate upload status.</span></span>|
|<span data-ttu-id="58a71-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="58a71-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="58a71-152">String</span><span class="sxs-lookup"><span data-stu-id="58a71-152">String</span></span>|<span data-ttu-id="58a71-153">原因证书上载失败。</span><span class="sxs-lookup"><span data-stu-id="58a71-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="58a71-154">certificate</span><span class="sxs-lookup"><span data-stu-id="58a71-154">certificate</span></span>|<span data-ttu-id="58a71-155">String</span><span class="sxs-lookup"><span data-stu-id="58a71-155">String</span></span>|<span data-ttu-id="58a71-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="58a71-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58a71-157">响应</span><span class="sxs-lookup"><span data-stu-id="58a71-157">Response</span></span>
<span data-ttu-id="58a71-158">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58a71-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a71-159">示例</span><span class="sxs-lookup"><span data-stu-id="58a71-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a71-160">请求</span><span class="sxs-lookup"><span data-stu-id="58a71-160">Request</span></span>
<span data-ttu-id="58a71-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58a71-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="58a71-162">响应</span><span class="sxs-lookup"><span data-stu-id="58a71-162">Response</span></span>
<span data-ttu-id="58a71-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58a71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





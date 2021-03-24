---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d5c82bd86b931fa619b0e92239558126df3ae0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136494"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="a6c82-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a6c82-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="a6c82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6c82-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6c82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6c82-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6c82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6c82-107">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6c82-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6c82-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6c82-108">Prerequisites</span></span>
<span data-ttu-id="a6c82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c82-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6c82-111">Permission type</span></span>|<span data-ttu-id="a6c82-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6c82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c82-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c82-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c82-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c82-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c82-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6c82-116">Not supported.</span></span>|
|<span data-ttu-id="a6c82-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6c82-117">Application</span></span>|<span data-ttu-id="a6c82-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c82-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c82-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6c82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a6c82-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6c82-120">Request headers</span></span>
|<span data-ttu-id="a6c82-121">标头</span><span class="sxs-lookup"><span data-stu-id="a6c82-121">Header</span></span>|<span data-ttu-id="a6c82-122">值</span><span class="sxs-lookup"><span data-stu-id="a6c82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c82-123">Authorization</span></span>|<span data-ttu-id="a6c82-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6c82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c82-125">接受</span><span class="sxs-lookup"><span data-stu-id="a6c82-125">Accept</span></span>|<span data-ttu-id="a6c82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c82-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6c82-127">Request body</span></span>
<span data-ttu-id="a6c82-128">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6c82-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="a6c82-129">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6c82-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="a6c82-130">属性</span><span class="sxs-lookup"><span data-stu-id="a6c82-130">Property</span></span>|<span data-ttu-id="a6c82-131">类型</span><span class="sxs-lookup"><span data-stu-id="a6c82-131">Type</span></span>|<span data-ttu-id="a6c82-132">说明</span><span class="sxs-lookup"><span data-stu-id="a6c82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c82-133">id</span><span class="sxs-lookup"><span data-stu-id="a6c82-133">id</span></span>|<span data-ttu-id="a6c82-134">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-134">String</span></span>|<span data-ttu-id="a6c82-135">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a6c82-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a6c82-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a6c82-136">appleIdentifier</span></span>|<span data-ttu-id="a6c82-137">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-137">String</span></span>|<span data-ttu-id="a6c82-138">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a6c82-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a6c82-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a6c82-139">topicIdentifier</span></span>|<span data-ttu-id="a6c82-140">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-140">String</span></span>|<span data-ttu-id="a6c82-141">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="a6c82-141">Topic Id.</span></span>|
|<span data-ttu-id="a6c82-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c82-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a6c82-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c82-143">DateTimeOffset</span></span>|<span data-ttu-id="a6c82-144">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a6c82-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a6c82-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c82-145">expirationDateTime</span></span>|<span data-ttu-id="a6c82-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c82-146">DateTimeOffset</span></span>|<span data-ttu-id="a6c82-147">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a6c82-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a6c82-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a6c82-148">certificateUploadStatus</span></span>|<span data-ttu-id="a6c82-149">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-149">String</span></span>|<span data-ttu-id="a6c82-150">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="a6c82-150">The certificate upload status.</span></span>|
|<span data-ttu-id="a6c82-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="a6c82-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="a6c82-152">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-152">String</span></span>|<span data-ttu-id="a6c82-153">证书上载失败的原因。</span><span class="sxs-lookup"><span data-stu-id="a6c82-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="a6c82-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a6c82-154">certificateSerialNumber</span></span>|<span data-ttu-id="a6c82-155">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-155">String</span></span>|<span data-ttu-id="a6c82-156">证书序列号。</span><span class="sxs-lookup"><span data-stu-id="a6c82-156">Certificate serial number.</span></span> <span data-ttu-id="a6c82-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a6c82-157">This property is read-only.</span></span>|
|<span data-ttu-id="a6c82-158">证书</span><span class="sxs-lookup"><span data-stu-id="a6c82-158">certificate</span></span>|<span data-ttu-id="a6c82-159">String</span><span class="sxs-lookup"><span data-stu-id="a6c82-159">String</span></span>|<span data-ttu-id="a6c82-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6c82-160">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6c82-161">响应</span><span class="sxs-lookup"><span data-stu-id="a6c82-161">Response</span></span>
<span data-ttu-id="a6c82-162">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6c82-162">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c82-163">示例</span><span class="sxs-lookup"><span data-stu-id="a6c82-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6c82-164">请求</span><span class="sxs-lookup"><span data-stu-id="a6c82-164">Request</span></span>
<span data-ttu-id="a6c82-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6c82-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="a6c82-166">响应</span><span class="sxs-lookup"><span data-stu-id="a6c82-166">Response</span></span>
<span data-ttu-id="a6c82-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6c82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```





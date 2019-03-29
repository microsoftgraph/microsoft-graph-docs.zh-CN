---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c16718f06b3f321e3a63180a1ee5155cf39de5a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981256"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="83393-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="83393-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="83393-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83393-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83393-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83393-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83393-106">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83393-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83393-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="83393-107">Prerequisites</span></span>
<span data-ttu-id="83393-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83393-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83393-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83393-110">Permission type</span></span>|<span data-ttu-id="83393-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83393-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83393-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83393-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83393-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83393-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="83393-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83393-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83393-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83393-115">Not supported.</span></span>|
|<span data-ttu-id="83393-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="83393-116">Application</span></span>|<span data-ttu-id="83393-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="83393-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83393-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83393-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="83393-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="83393-119">Request headers</span></span>
|<span data-ttu-id="83393-120">标头</span><span class="sxs-lookup"><span data-stu-id="83393-120">Header</span></span>|<span data-ttu-id="83393-121">值</span><span class="sxs-lookup"><span data-stu-id="83393-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83393-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83393-122">Authorization</span></span>|<span data-ttu-id="83393-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83393-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83393-124">接受</span><span class="sxs-lookup"><span data-stu-id="83393-124">Accept</span></span>|<span data-ttu-id="83393-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83393-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83393-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="83393-126">Request body</span></span>
<span data-ttu-id="83393-127">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83393-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="83393-128">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83393-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="83393-129">属性</span><span class="sxs-lookup"><span data-stu-id="83393-129">Property</span></span>|<span data-ttu-id="83393-130">类型</span><span class="sxs-lookup"><span data-stu-id="83393-130">Type</span></span>|<span data-ttu-id="83393-131">说明</span><span class="sxs-lookup"><span data-stu-id="83393-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83393-132">id</span><span class="sxs-lookup"><span data-stu-id="83393-132">id</span></span>|<span data-ttu-id="83393-133">String</span><span class="sxs-lookup"><span data-stu-id="83393-133">String</span></span>|<span data-ttu-id="83393-134">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="83393-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="83393-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="83393-135">appleIdentifier</span></span>|<span data-ttu-id="83393-136">String</span><span class="sxs-lookup"><span data-stu-id="83393-136">String</span></span>|<span data-ttu-id="83393-137">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="83393-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="83393-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="83393-138">topicIdentifier</span></span>|<span data-ttu-id="83393-139">String</span><span class="sxs-lookup"><span data-stu-id="83393-139">String</span></span>|<span data-ttu-id="83393-140">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="83393-140">Topic Id.</span></span>|
|<span data-ttu-id="83393-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83393-141">lastModifiedDateTime</span></span>|<span data-ttu-id="83393-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83393-142">DateTimeOffset</span></span>|<span data-ttu-id="83393-143">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="83393-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="83393-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="83393-144">expirationDateTime</span></span>|<span data-ttu-id="83393-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83393-145">DateTimeOffset</span></span>|<span data-ttu-id="83393-146">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="83393-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="83393-147">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="83393-147">certificateUploadStatus</span></span>|<span data-ttu-id="83393-148">String</span><span class="sxs-lookup"><span data-stu-id="83393-148">String</span></span>|<span data-ttu-id="83393-149">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="83393-149">The certificate upload status.</span></span>|
|<span data-ttu-id="83393-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="83393-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="83393-151">String</span><span class="sxs-lookup"><span data-stu-id="83393-151">String</span></span>|<span data-ttu-id="83393-152">证书上传失败的原因。</span><span class="sxs-lookup"><span data-stu-id="83393-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="83393-153">证书</span><span class="sxs-lookup"><span data-stu-id="83393-153">certificate</span></span>|<span data-ttu-id="83393-154">String</span><span class="sxs-lookup"><span data-stu-id="83393-154">String</span></span>|<span data-ttu-id="83393-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="83393-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83393-156">响应</span><span class="sxs-lookup"><span data-stu-id="83393-156">Response</span></span>
<span data-ttu-id="83393-157">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83393-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83393-158">示例</span><span class="sxs-lookup"><span data-stu-id="83393-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="83393-159">请求</span><span class="sxs-lookup"><span data-stu-id="83393-159">Request</span></span>
<span data-ttu-id="83393-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83393-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83393-161">响应</span><span class="sxs-lookup"><span data-stu-id="83393-161">Response</span></span>
<span data-ttu-id="83393-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83393-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





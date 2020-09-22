---
title: 更新 applePushNotificationCertificate
description: 更新 applePushNotificationCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b26db969076896a8fb45dbe8d2c06894e50d0a9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009623"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="ff3c2-103">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ff3c2-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="ff3c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff3c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff3c2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff3c2-106">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff3c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff3c2-107">Prerequisites</span></span>
<span data-ttu-id="ff3c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff3c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff3c2-110">Permission type</span></span>|<span data-ttu-id="ff3c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff3c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff3c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff3c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff3c2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff3c2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff3c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff3c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff3c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-115">Not supported.</span></span>|
|<span data-ttu-id="ff3c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff3c2-116">Application</span></span>|<span data-ttu-id="ff3c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff3c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff3c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="ff3c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff3c2-119">Request headers</span></span>
|<span data-ttu-id="ff3c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="ff3c2-120">Header</span></span>|<span data-ttu-id="ff3c2-121">值</span><span class="sxs-lookup"><span data-stu-id="ff3c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff3c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff3c2-122">Authorization</span></span>|<span data-ttu-id="ff3c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff3c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="ff3c2-124">Accept</span></span>|<span data-ttu-id="ff3c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff3c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff3c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff3c2-126">Request body</span></span>
<span data-ttu-id="ff3c2-127">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="ff3c2-128">下表显示创建 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="ff3c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff3c2-129">Property</span></span>|<span data-ttu-id="ff3c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="ff3c2-130">Type</span></span>|<span data-ttu-id="ff3c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="ff3c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3c2-132">id</span><span class="sxs-lookup"><span data-stu-id="ff3c2-132">id</span></span>|<span data-ttu-id="ff3c2-133">String</span><span class="sxs-lookup"><span data-stu-id="ff3c2-133">String</span></span>|<span data-ttu-id="ff3c2-134">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ff3c2-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="ff3c2-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff3c2-135">appleIdentifier</span></span>|<span data-ttu-id="ff3c2-136">String</span><span class="sxs-lookup"><span data-stu-id="ff3c2-136">String</span></span>|<span data-ttu-id="ff3c2-137">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="ff3c2-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff3c2-138">topicIdentifier</span></span>|<span data-ttu-id="ff3c2-139">String</span><span class="sxs-lookup"><span data-stu-id="ff3c2-139">String</span></span>|<span data-ttu-id="ff3c2-140">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-140">Topic Id.</span></span>|
|<span data-ttu-id="ff3c2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff3c2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ff3c2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff3c2-142">DateTimeOffset</span></span>|<span data-ttu-id="ff3c2-143">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ff3c2-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ff3c2-144">expirationDateTime</span></span>|<span data-ttu-id="ff3c2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff3c2-145">DateTimeOffset</span></span>|<span data-ttu-id="ff3c2-146">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ff3c2-147">证书</span><span class="sxs-lookup"><span data-stu-id="ff3c2-147">certificate</span></span>|<span data-ttu-id="ff3c2-148">String</span><span class="sxs-lookup"><span data-stu-id="ff3c2-148">String</span></span>|<span data-ttu-id="ff3c2-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff3c2-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff3c2-150">响应</span><span class="sxs-lookup"><span data-stu-id="ff3c2-150">Response</span></span>
<span data-ttu-id="ff3c2-151">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff3c2-152">示例</span><span class="sxs-lookup"><span data-stu-id="ff3c2-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff3c2-153">请求</span><span class="sxs-lookup"><span data-stu-id="ff3c2-153">Request</span></span>
<span data-ttu-id="ff3c2-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff3c2-155">响应</span><span class="sxs-lookup"><span data-stu-id="ff3c2-155">Response</span></span>
<span data-ttu-id="ff3c2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff3c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










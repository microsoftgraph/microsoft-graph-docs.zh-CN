---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 63e4b858404242d84597a7f650bae6c0870f5b76
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162503"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="917e7-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="917e7-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="917e7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="917e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="917e7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="917e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="917e7-106">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="917e7-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="917e7-107">方法</span><span class="sxs-lookup"><span data-stu-id="917e7-107">Methods</span></span>
|<span data-ttu-id="917e7-108">方法</span><span class="sxs-lookup"><span data-stu-id="917e7-108">Method</span></span>|<span data-ttu-id="917e7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="917e7-109">Return Type</span></span>|<span data-ttu-id="917e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="917e7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="917e7-111">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="917e7-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="917e7-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="917e7-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="917e7-113">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="917e7-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="917e7-114">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="917e7-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="917e7-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="917e7-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="917e7-116">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="917e7-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="917e7-117">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="917e7-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="917e7-118">String</span><span class="sxs-lookup"><span data-stu-id="917e7-118">String</span></span>|<span data-ttu-id="917e7-119">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="917e7-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="917e7-120">属性</span><span class="sxs-lookup"><span data-stu-id="917e7-120">Properties</span></span>
|<span data-ttu-id="917e7-121">属性</span><span class="sxs-lookup"><span data-stu-id="917e7-121">Property</span></span>|<span data-ttu-id="917e7-122">类型</span><span class="sxs-lookup"><span data-stu-id="917e7-122">Type</span></span>|<span data-ttu-id="917e7-123">说明</span><span class="sxs-lookup"><span data-stu-id="917e7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="917e7-124">id</span><span class="sxs-lookup"><span data-stu-id="917e7-124">id</span></span>|<span data-ttu-id="917e7-125">String</span><span class="sxs-lookup"><span data-stu-id="917e7-125">String</span></span>|<span data-ttu-id="917e7-126">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="917e7-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="917e7-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="917e7-127">appleIdentifier</span></span>|<span data-ttu-id="917e7-128">String</span><span class="sxs-lookup"><span data-stu-id="917e7-128">String</span></span>|<span data-ttu-id="917e7-129">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="917e7-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="917e7-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="917e7-130">topicIdentifier</span></span>|<span data-ttu-id="917e7-131">String</span><span class="sxs-lookup"><span data-stu-id="917e7-131">String</span></span>|<span data-ttu-id="917e7-132">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="917e7-132">Topic Id.</span></span>|
|<span data-ttu-id="917e7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="917e7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="917e7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917e7-134">DateTimeOffset</span></span>|<span data-ttu-id="917e7-135">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="917e7-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="917e7-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="917e7-136">expirationDateTime</span></span>|<span data-ttu-id="917e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917e7-137">DateTimeOffset</span></span>|<span data-ttu-id="917e7-138">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="917e7-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="917e7-139">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="917e7-139">certificateUploadStatus</span></span>|<span data-ttu-id="917e7-140">String</span><span class="sxs-lookup"><span data-stu-id="917e7-140">String</span></span>|<span data-ttu-id="917e7-141">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="917e7-141">The certificate upload status.</span></span>|
|<span data-ttu-id="917e7-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="917e7-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="917e7-143">String</span><span class="sxs-lookup"><span data-stu-id="917e7-143">String</span></span>|<span data-ttu-id="917e7-144">证书上传失败的原因。</span><span class="sxs-lookup"><span data-stu-id="917e7-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="917e7-145">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="917e7-145">certificateSerialNumber</span></span>|<span data-ttu-id="917e7-146">String</span><span class="sxs-lookup"><span data-stu-id="917e7-146">String</span></span>|<span data-ttu-id="917e7-147">证书序列号。</span><span class="sxs-lookup"><span data-stu-id="917e7-147">Certificate serial number.</span></span> <span data-ttu-id="917e7-148">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="917e7-148">This property is read-only.</span></span>|
|<span data-ttu-id="917e7-149">证书</span><span class="sxs-lookup"><span data-stu-id="917e7-149">certificate</span></span>|<span data-ttu-id="917e7-150">String</span><span class="sxs-lookup"><span data-stu-id="917e7-150">String</span></span>|<span data-ttu-id="917e7-151">尚未记录</span><span class="sxs-lookup"><span data-stu-id="917e7-151">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="917e7-152">关系</span><span class="sxs-lookup"><span data-stu-id="917e7-152">Relationships</span></span>
<span data-ttu-id="917e7-153">无</span><span class="sxs-lookup"><span data-stu-id="917e7-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="917e7-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="917e7-154">JSON Representation</span></span>
<span data-ttu-id="917e7-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="917e7-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```




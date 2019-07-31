---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d4a5725c6cd046c4baa34316f74a90b4c9fb05f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000044"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="cc656-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc656-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="cc656-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc656-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc656-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc656-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc656-106">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="cc656-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="cc656-107">方法</span><span class="sxs-lookup"><span data-stu-id="cc656-107">Methods</span></span>
|<span data-ttu-id="cc656-108">方法</span><span class="sxs-lookup"><span data-stu-id="cc656-108">Method</span></span>|<span data-ttu-id="cc656-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc656-109">Return Type</span></span>|<span data-ttu-id="cc656-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc656-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc656-111">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cc656-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="cc656-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cc656-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="cc656-113">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc656-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="cc656-114">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cc656-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="cc656-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cc656-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="cc656-116">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cc656-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="cc656-117">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="cc656-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="cc656-118">String</span><span class="sxs-lookup"><span data-stu-id="cc656-118">String</span></span>|<span data-ttu-id="cc656-119">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="cc656-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="cc656-120">属性</span><span class="sxs-lookup"><span data-stu-id="cc656-120">Properties</span></span>
|<span data-ttu-id="cc656-121">属性</span><span class="sxs-lookup"><span data-stu-id="cc656-121">Property</span></span>|<span data-ttu-id="cc656-122">类型</span><span class="sxs-lookup"><span data-stu-id="cc656-122">Type</span></span>|<span data-ttu-id="cc656-123">说明</span><span class="sxs-lookup"><span data-stu-id="cc656-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc656-124">id</span><span class="sxs-lookup"><span data-stu-id="cc656-124">id</span></span>|<span data-ttu-id="cc656-125">String</span><span class="sxs-lookup"><span data-stu-id="cc656-125">String</span></span>|<span data-ttu-id="cc656-126">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cc656-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="cc656-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc656-127">appleIdentifier</span></span>|<span data-ttu-id="cc656-128">String</span><span class="sxs-lookup"><span data-stu-id="cc656-128">String</span></span>|<span data-ttu-id="cc656-129">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="cc656-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="cc656-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc656-130">topicIdentifier</span></span>|<span data-ttu-id="cc656-131">String</span><span class="sxs-lookup"><span data-stu-id="cc656-131">String</span></span>|<span data-ttu-id="cc656-132">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="cc656-132">Topic Id.</span></span>|
|<span data-ttu-id="cc656-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc656-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cc656-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc656-134">DateTimeOffset</span></span>|<span data-ttu-id="cc656-135">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc656-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="cc656-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc656-136">expirationDateTime</span></span>|<span data-ttu-id="cc656-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc656-137">DateTimeOffset</span></span>|<span data-ttu-id="cc656-138">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc656-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="cc656-139">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="cc656-139">certificateUploadStatus</span></span>|<span data-ttu-id="cc656-140">String</span><span class="sxs-lookup"><span data-stu-id="cc656-140">String</span></span>|<span data-ttu-id="cc656-141">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="cc656-141">The certificate upload status.</span></span>|
|<span data-ttu-id="cc656-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="cc656-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="cc656-143">String</span><span class="sxs-lookup"><span data-stu-id="cc656-143">String</span></span>|<span data-ttu-id="cc656-144">证书上传失败的原因。</span><span class="sxs-lookup"><span data-stu-id="cc656-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="cc656-145">证书</span><span class="sxs-lookup"><span data-stu-id="cc656-145">certificate</span></span>|<span data-ttu-id="cc656-146">String</span><span class="sxs-lookup"><span data-stu-id="cc656-146">String</span></span>|<span data-ttu-id="cc656-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cc656-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc656-148">关系</span><span class="sxs-lookup"><span data-stu-id="cc656-148">Relationships</span></span>
<span data-ttu-id="cc656-149">无</span><span class="sxs-lookup"><span data-stu-id="cc656-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc656-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc656-150">JSON Representation</span></span>
<span data-ttu-id="cc656-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc656-151">Here is a JSON representation of the resource.</span></span>
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
  "certificate": "String"
}
```






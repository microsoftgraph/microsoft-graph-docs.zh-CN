---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8a5df851f1826cd3e1e124bf8c2cda89b24da8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395585"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="38dfc-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="38dfc-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="38dfc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="38dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38dfc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38dfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38dfc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38dfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38dfc-107">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="38dfc-107">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="38dfc-108">方法</span><span class="sxs-lookup"><span data-stu-id="38dfc-108">Methods</span></span>
|<span data-ttu-id="38dfc-109">方法</span><span class="sxs-lookup"><span data-stu-id="38dfc-109">Method</span></span>|<span data-ttu-id="38dfc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="38dfc-110">Return Type</span></span>|<span data-ttu-id="38dfc-111">说明</span><span class="sxs-lookup"><span data-stu-id="38dfc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38dfc-112">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="38dfc-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="38dfc-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="38dfc-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="38dfc-114">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38dfc-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="38dfc-115">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="38dfc-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="38dfc-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="38dfc-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="38dfc-117">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38dfc-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="38dfc-118">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="38dfc-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="38dfc-119">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-119">String</span></span>|<span data-ttu-id="38dfc-120">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="38dfc-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="38dfc-121">属性</span><span class="sxs-lookup"><span data-stu-id="38dfc-121">Properties</span></span>
|<span data-ttu-id="38dfc-122">属性</span><span class="sxs-lookup"><span data-stu-id="38dfc-122">Property</span></span>|<span data-ttu-id="38dfc-123">类型</span><span class="sxs-lookup"><span data-stu-id="38dfc-123">Type</span></span>|<span data-ttu-id="38dfc-124">说明</span><span class="sxs-lookup"><span data-stu-id="38dfc-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38dfc-125">id</span><span class="sxs-lookup"><span data-stu-id="38dfc-125">id</span></span>|<span data-ttu-id="38dfc-126">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-126">String</span></span>|<span data-ttu-id="38dfc-127">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="38dfc-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="38dfc-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="38dfc-128">appleIdentifier</span></span>|<span data-ttu-id="38dfc-129">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-129">String</span></span>|<span data-ttu-id="38dfc-130">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="38dfc-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="38dfc-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="38dfc-131">topicIdentifier</span></span>|<span data-ttu-id="38dfc-132">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-132">String</span></span>|<span data-ttu-id="38dfc-133">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="38dfc-133">Topic Id.</span></span>|
|<span data-ttu-id="38dfc-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38dfc-134">lastModifiedDateTime</span></span>|<span data-ttu-id="38dfc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38dfc-135">DateTimeOffset</span></span>|<span data-ttu-id="38dfc-136">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="38dfc-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="38dfc-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="38dfc-137">expirationDateTime</span></span>|<span data-ttu-id="38dfc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38dfc-138">DateTimeOffset</span></span>|<span data-ttu-id="38dfc-139">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="38dfc-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="38dfc-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="38dfc-140">certificateUploadStatus</span></span>|<span data-ttu-id="38dfc-141">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-141">String</span></span>|<span data-ttu-id="38dfc-142">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="38dfc-142">The certificate upload status.</span></span>|
|<span data-ttu-id="38dfc-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="38dfc-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="38dfc-144">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-144">String</span></span>|<span data-ttu-id="38dfc-145">原因证书上载失败。</span><span class="sxs-lookup"><span data-stu-id="38dfc-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="38dfc-146">certificate</span><span class="sxs-lookup"><span data-stu-id="38dfc-146">certificate</span></span>|<span data-ttu-id="38dfc-147">String</span><span class="sxs-lookup"><span data-stu-id="38dfc-147">String</span></span>|<span data-ttu-id="38dfc-148">尚未记录</span><span class="sxs-lookup"><span data-stu-id="38dfc-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="38dfc-149">关系</span><span class="sxs-lookup"><span data-stu-id="38dfc-149">Relationships</span></span>
<span data-ttu-id="38dfc-150">无</span><span class="sxs-lookup"><span data-stu-id="38dfc-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38dfc-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38dfc-151">JSON Representation</span></span>
<span data-ttu-id="38dfc-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38dfc-152">Here is a JSON representation of the resource.</span></span>
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





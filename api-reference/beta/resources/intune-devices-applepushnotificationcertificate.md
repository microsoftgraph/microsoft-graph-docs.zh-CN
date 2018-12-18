---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: tfitzmac
ms.openlocfilehash: 11c03712cc482a882452a9b64867090260863075
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306648"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="01192-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="01192-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="01192-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01192-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01192-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01192-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01192-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="01192-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01192-107">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="01192-107">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="01192-108">方法</span><span class="sxs-lookup"><span data-stu-id="01192-108">Methods</span></span>
|<span data-ttu-id="01192-109">方法</span><span class="sxs-lookup"><span data-stu-id="01192-109">Method</span></span>|<span data-ttu-id="01192-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="01192-110">Return Type</span></span>|<span data-ttu-id="01192-111">说明</span><span class="sxs-lookup"><span data-stu-id="01192-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01192-112">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="01192-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="01192-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="01192-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="01192-114">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01192-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="01192-115">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="01192-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="01192-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="01192-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="01192-117">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="01192-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="01192-118">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="01192-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="01192-119">String</span><span class="sxs-lookup"><span data-stu-id="01192-119">String</span></span>|<span data-ttu-id="01192-120">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="01192-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="01192-121">属性</span><span class="sxs-lookup"><span data-stu-id="01192-121">Properties</span></span>
|<span data-ttu-id="01192-122">属性</span><span class="sxs-lookup"><span data-stu-id="01192-122">Property</span></span>|<span data-ttu-id="01192-123">类型</span><span class="sxs-lookup"><span data-stu-id="01192-123">Type</span></span>|<span data-ttu-id="01192-124">说明</span><span class="sxs-lookup"><span data-stu-id="01192-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01192-125">id</span><span class="sxs-lookup"><span data-stu-id="01192-125">id</span></span>|<span data-ttu-id="01192-126">String</span><span class="sxs-lookup"><span data-stu-id="01192-126">String</span></span>|<span data-ttu-id="01192-127">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="01192-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="01192-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="01192-128">appleIdentifier</span></span>|<span data-ttu-id="01192-129">String</span><span class="sxs-lookup"><span data-stu-id="01192-129">String</span></span>|<span data-ttu-id="01192-130">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="01192-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="01192-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="01192-131">topicIdentifier</span></span>|<span data-ttu-id="01192-132">String</span><span class="sxs-lookup"><span data-stu-id="01192-132">String</span></span>|<span data-ttu-id="01192-133">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="01192-133">Topic Id.</span></span>|
|<span data-ttu-id="01192-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01192-134">lastModifiedDateTime</span></span>|<span data-ttu-id="01192-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01192-135">DateTimeOffset</span></span>|<span data-ttu-id="01192-136">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="01192-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="01192-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="01192-137">expirationDateTime</span></span>|<span data-ttu-id="01192-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01192-138">DateTimeOffset</span></span>|<span data-ttu-id="01192-139">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="01192-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="01192-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="01192-140">certificateUploadStatus</span></span>|<span data-ttu-id="01192-141">字符串</span><span class="sxs-lookup"><span data-stu-id="01192-141">String</span></span>|<span data-ttu-id="01192-142">证书上载状态。</span><span class="sxs-lookup"><span data-stu-id="01192-142">The certificate upload status.</span></span>|
|<span data-ttu-id="01192-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="01192-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="01192-144">字符串</span><span class="sxs-lookup"><span data-stu-id="01192-144">String</span></span>|<span data-ttu-id="01192-145">原因证书上载失败。</span><span class="sxs-lookup"><span data-stu-id="01192-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="01192-146">certificate</span><span class="sxs-lookup"><span data-stu-id="01192-146">certificate</span></span>|<span data-ttu-id="01192-147">String</span><span class="sxs-lookup"><span data-stu-id="01192-147">String</span></span>|<span data-ttu-id="01192-148">尚未记录</span><span class="sxs-lookup"><span data-stu-id="01192-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="01192-149">关系</span><span class="sxs-lookup"><span data-stu-id="01192-149">Relationships</span></span>
<span data-ttu-id="01192-150">无</span><span class="sxs-lookup"><span data-stu-id="01192-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01192-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01192-151">JSON Representation</span></span>
<span data-ttu-id="01192-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01192-152">Here is a JSON representation of the resource.</span></span>
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






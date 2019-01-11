---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43a697feaab14589540747ff0f4f79ca194918ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856839"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="5c9cf-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c9cf-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="5c9cf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c9cf-105">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="5c9cf-106">方法</span><span class="sxs-lookup"><span data-stu-id="5c9cf-106">Methods</span></span>
|<span data-ttu-id="5c9cf-107">方法</span><span class="sxs-lookup"><span data-stu-id="5c9cf-107">Method</span></span>|<span data-ttu-id="5c9cf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c9cf-108">Return Type</span></span>|<span data-ttu-id="5c9cf-109">说明</span><span class="sxs-lookup"><span data-stu-id="5c9cf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c9cf-110">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5c9cf-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="5c9cf-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5c9cf-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="5c9cf-112">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="5c9cf-113">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5c9cf-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="5c9cf-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5c9cf-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="5c9cf-115">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="5c9cf-116">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="5c9cf-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="5c9cf-117">String</span><span class="sxs-lookup"><span data-stu-id="5c9cf-117">String</span></span>|<span data-ttu-id="5c9cf-118">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="5c9cf-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="5c9cf-119">属性</span><span class="sxs-lookup"><span data-stu-id="5c9cf-119">Properties</span></span>
|<span data-ttu-id="5c9cf-120">属性</span><span class="sxs-lookup"><span data-stu-id="5c9cf-120">Property</span></span>|<span data-ttu-id="5c9cf-121">类型</span><span class="sxs-lookup"><span data-stu-id="5c9cf-121">Type</span></span>|<span data-ttu-id="5c9cf-122">说明</span><span class="sxs-lookup"><span data-stu-id="5c9cf-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c9cf-123">id</span><span class="sxs-lookup"><span data-stu-id="5c9cf-123">id</span></span>|<span data-ttu-id="5c9cf-124">String</span><span class="sxs-lookup"><span data-stu-id="5c9cf-124">String</span></span>|<span data-ttu-id="5c9cf-125">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5c9cf-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5c9cf-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c9cf-126">appleIdentifier</span></span>|<span data-ttu-id="5c9cf-127">String</span><span class="sxs-lookup"><span data-stu-id="5c9cf-127">String</span></span>|<span data-ttu-id="5c9cf-128">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5c9cf-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c9cf-129">topicIdentifier</span></span>|<span data-ttu-id="5c9cf-130">String</span><span class="sxs-lookup"><span data-stu-id="5c9cf-130">String</span></span>|<span data-ttu-id="5c9cf-131">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-131">Topic Id.</span></span>|
|<span data-ttu-id="5c9cf-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c9cf-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5c9cf-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c9cf-133">DateTimeOffset</span></span>|<span data-ttu-id="5c9cf-134">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5c9cf-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5c9cf-135">expirationDateTime</span></span>|<span data-ttu-id="5c9cf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c9cf-136">DateTimeOffset</span></span>|<span data-ttu-id="5c9cf-137">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5c9cf-138">certificate</span><span class="sxs-lookup"><span data-stu-id="5c9cf-138">certificate</span></span>|<span data-ttu-id="5c9cf-139">String</span><span class="sxs-lookup"><span data-stu-id="5c9cf-139">String</span></span>|<span data-ttu-id="5c9cf-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c9cf-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c9cf-141">关系</span><span class="sxs-lookup"><span data-stu-id="5c9cf-141">Relationships</span></span>
<span data-ttu-id="5c9cf-142">无</span><span class="sxs-lookup"><span data-stu-id="5c9cf-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c9cf-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c9cf-143">JSON Representation</span></span>
<span data-ttu-id="5c9cf-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c9cf-144">Here is a JSON representation of the resource.</span></span>
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
  "certificate": "String"
}
```




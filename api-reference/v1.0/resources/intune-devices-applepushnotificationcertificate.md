---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 511e70f2ccbb5c79f3b00e0027a62dd9542f0669
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357071"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="b1812-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1812-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="b1812-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1812-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1812-105">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="b1812-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="b1812-106">方法</span><span class="sxs-lookup"><span data-stu-id="b1812-106">Methods</span></span>
|<span data-ttu-id="b1812-107">方法</span><span class="sxs-lookup"><span data-stu-id="b1812-107">Method</span></span>|<span data-ttu-id="b1812-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1812-108">Return Type</span></span>|<span data-ttu-id="b1812-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1812-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1812-110">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b1812-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="b1812-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b1812-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="b1812-112">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1812-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="b1812-113">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b1812-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="b1812-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b1812-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="b1812-115">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1812-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="b1812-116">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="b1812-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="b1812-117">String</span><span class="sxs-lookup"><span data-stu-id="b1812-117">String</span></span>|<span data-ttu-id="b1812-118">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="b1812-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="b1812-119">属性</span><span class="sxs-lookup"><span data-stu-id="b1812-119">Properties</span></span>
|<span data-ttu-id="b1812-120">属性</span><span class="sxs-lookup"><span data-stu-id="b1812-120">Property</span></span>|<span data-ttu-id="b1812-121">类型</span><span class="sxs-lookup"><span data-stu-id="b1812-121">Type</span></span>|<span data-ttu-id="b1812-122">说明</span><span class="sxs-lookup"><span data-stu-id="b1812-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1812-123">id</span><span class="sxs-lookup"><span data-stu-id="b1812-123">id</span></span>|<span data-ttu-id="b1812-124">String</span><span class="sxs-lookup"><span data-stu-id="b1812-124">String</span></span>|<span data-ttu-id="b1812-125">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b1812-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b1812-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1812-126">appleIdentifier</span></span>|<span data-ttu-id="b1812-127">String</span><span class="sxs-lookup"><span data-stu-id="b1812-127">String</span></span>|<span data-ttu-id="b1812-128">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b1812-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b1812-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1812-129">topicIdentifier</span></span>|<span data-ttu-id="b1812-130">String</span><span class="sxs-lookup"><span data-stu-id="b1812-130">String</span></span>|<span data-ttu-id="b1812-131">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="b1812-131">Topic Id.</span></span>|
|<span data-ttu-id="b1812-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1812-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b1812-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1812-133">DateTimeOffset</span></span>|<span data-ttu-id="b1812-134">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b1812-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b1812-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1812-135">expirationDateTime</span></span>|<span data-ttu-id="b1812-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1812-136">DateTimeOffset</span></span>|<span data-ttu-id="b1812-137">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b1812-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b1812-138">证书</span><span class="sxs-lookup"><span data-stu-id="b1812-138">certificate</span></span>|<span data-ttu-id="b1812-139">String</span><span class="sxs-lookup"><span data-stu-id="b1812-139">String</span></span>|<span data-ttu-id="b1812-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1812-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1812-141">关系</span><span class="sxs-lookup"><span data-stu-id="b1812-141">Relationships</span></span>
<span data-ttu-id="b1812-142">无</span><span class="sxs-lookup"><span data-stu-id="b1812-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1812-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1812-143">JSON Representation</span></span>
<span data-ttu-id="b1812-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1812-144">Here is a JSON representation of the resource.</span></span>
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





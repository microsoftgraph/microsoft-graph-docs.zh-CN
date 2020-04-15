---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79c7bcd1bfe7a1eac1820cbe7163cac0b2b5311e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451314"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="ceba3-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="ceba3-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="ceba3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceba3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceba3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ceba3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceba3-106">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="ceba3-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="ceba3-107">方法</span><span class="sxs-lookup"><span data-stu-id="ceba3-107">Methods</span></span>
|<span data-ttu-id="ceba3-108">方法</span><span class="sxs-lookup"><span data-stu-id="ceba3-108">Method</span></span>|<span data-ttu-id="ceba3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ceba3-109">Return Type</span></span>|<span data-ttu-id="ceba3-110">说明</span><span class="sxs-lookup"><span data-stu-id="ceba3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ceba3-111">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ceba3-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="ceba3-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ceba3-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ceba3-113">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ceba3-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ceba3-114">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ceba3-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="ceba3-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ceba3-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ceba3-116">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ceba3-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ceba3-117">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="ceba3-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="ceba3-118">String</span><span class="sxs-lookup"><span data-stu-id="ceba3-118">String</span></span>|<span data-ttu-id="ceba3-119">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="ceba3-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="ceba3-120">属性</span><span class="sxs-lookup"><span data-stu-id="ceba3-120">Properties</span></span>
|<span data-ttu-id="ceba3-121">属性</span><span class="sxs-lookup"><span data-stu-id="ceba3-121">Property</span></span>|<span data-ttu-id="ceba3-122">类型</span><span class="sxs-lookup"><span data-stu-id="ceba3-122">Type</span></span>|<span data-ttu-id="ceba3-123">说明</span><span class="sxs-lookup"><span data-stu-id="ceba3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceba3-124">id</span><span class="sxs-lookup"><span data-stu-id="ceba3-124">id</span></span>|<span data-ttu-id="ceba3-125">String</span><span class="sxs-lookup"><span data-stu-id="ceba3-125">String</span></span>|<span data-ttu-id="ceba3-126">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ceba3-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="ceba3-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ceba3-127">appleIdentifier</span></span>|<span data-ttu-id="ceba3-128">String</span><span class="sxs-lookup"><span data-stu-id="ceba3-128">String</span></span>|<span data-ttu-id="ceba3-129">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ceba3-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="ceba3-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="ceba3-130">topicIdentifier</span></span>|<span data-ttu-id="ceba3-131">String</span><span class="sxs-lookup"><span data-stu-id="ceba3-131">String</span></span>|<span data-ttu-id="ceba3-132">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="ceba3-132">Topic Id.</span></span>|
|<span data-ttu-id="ceba3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceba3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ceba3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceba3-134">DateTimeOffset</span></span>|<span data-ttu-id="ceba3-135">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ceba3-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ceba3-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ceba3-136">expirationDateTime</span></span>|<span data-ttu-id="ceba3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceba3-137">DateTimeOffset</span></span>|<span data-ttu-id="ceba3-138">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ceba3-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ceba3-139">证书</span><span class="sxs-lookup"><span data-stu-id="ceba3-139">certificate</span></span>|<span data-ttu-id="ceba3-140">String</span><span class="sxs-lookup"><span data-stu-id="ceba3-140">String</span></span>|<span data-ttu-id="ceba3-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ceba3-141">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceba3-142">关系</span><span class="sxs-lookup"><span data-stu-id="ceba3-142">Relationships</span></span>
<span data-ttu-id="ceba3-143">无</span><span class="sxs-lookup"><span data-stu-id="ceba3-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceba3-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ceba3-144">JSON Representation</span></span>
<span data-ttu-id="ceba3-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceba3-145">Here is a JSON representation of the resource.</span></span>
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








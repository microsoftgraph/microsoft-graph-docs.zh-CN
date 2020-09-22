---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bbcca2707223f53b59d1b3d5d2ceb75ba08c57a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091318"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="3d015-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d015-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="3d015-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d015-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d015-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d015-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d015-106">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="3d015-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="3d015-107">方法</span><span class="sxs-lookup"><span data-stu-id="3d015-107">Methods</span></span>
|<span data-ttu-id="3d015-108">方法</span><span class="sxs-lookup"><span data-stu-id="3d015-108">Method</span></span>|<span data-ttu-id="3d015-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d015-109">Return Type</span></span>|<span data-ttu-id="3d015-110">说明</span><span class="sxs-lookup"><span data-stu-id="3d015-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d015-111">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3d015-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="3d015-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3d015-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="3d015-113">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d015-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="3d015-114">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3d015-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="3d015-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3d015-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="3d015-116">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d015-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="3d015-117">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="3d015-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="3d015-118">String</span><span class="sxs-lookup"><span data-stu-id="3d015-118">String</span></span>|<span data-ttu-id="3d015-119">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="3d015-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="3d015-120">属性</span><span class="sxs-lookup"><span data-stu-id="3d015-120">Properties</span></span>
|<span data-ttu-id="3d015-121">属性</span><span class="sxs-lookup"><span data-stu-id="3d015-121">Property</span></span>|<span data-ttu-id="3d015-122">类型</span><span class="sxs-lookup"><span data-stu-id="3d015-122">Type</span></span>|<span data-ttu-id="3d015-123">说明</span><span class="sxs-lookup"><span data-stu-id="3d015-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d015-124">id</span><span class="sxs-lookup"><span data-stu-id="3d015-124">id</span></span>|<span data-ttu-id="3d015-125">String</span><span class="sxs-lookup"><span data-stu-id="3d015-125">String</span></span>|<span data-ttu-id="3d015-126">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3d015-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="3d015-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d015-127">appleIdentifier</span></span>|<span data-ttu-id="3d015-128">String</span><span class="sxs-lookup"><span data-stu-id="3d015-128">String</span></span>|<span data-ttu-id="3d015-129">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="3d015-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="3d015-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d015-130">topicIdentifier</span></span>|<span data-ttu-id="3d015-131">String</span><span class="sxs-lookup"><span data-stu-id="3d015-131">String</span></span>|<span data-ttu-id="3d015-132">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="3d015-132">Topic Id.</span></span>|
|<span data-ttu-id="3d015-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d015-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3d015-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d015-134">DateTimeOffset</span></span>|<span data-ttu-id="3d015-135">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d015-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3d015-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d015-136">expirationDateTime</span></span>|<span data-ttu-id="3d015-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d015-137">DateTimeOffset</span></span>|<span data-ttu-id="3d015-138">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d015-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3d015-139">证书</span><span class="sxs-lookup"><span data-stu-id="3d015-139">certificate</span></span>|<span data-ttu-id="3d015-140">String</span><span class="sxs-lookup"><span data-stu-id="3d015-140">String</span></span>|<span data-ttu-id="3d015-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3d015-141">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d015-142">关系</span><span class="sxs-lookup"><span data-stu-id="3d015-142">Relationships</span></span>
<span data-ttu-id="3d015-143">无</span><span class="sxs-lookup"><span data-stu-id="3d015-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d015-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d015-144">JSON Representation</span></span>
<span data-ttu-id="3d015-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d015-145">Here is a JSON representation of the resource.</span></span>
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










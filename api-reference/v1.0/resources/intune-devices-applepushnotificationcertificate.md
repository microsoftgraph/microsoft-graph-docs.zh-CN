---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d53407d5ec380e7bfe11d50f6871eb6bbfb87aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760207"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="a1fa0-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1fa0-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="a1fa0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1fa0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1fa0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1fa0-106">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="a1fa0-107">方法</span><span class="sxs-lookup"><span data-stu-id="a1fa0-107">Methods</span></span>
|<span data-ttu-id="a1fa0-108">方法</span><span class="sxs-lookup"><span data-stu-id="a1fa0-108">Method</span></span>|<span data-ttu-id="a1fa0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1fa0-109">Return Type</span></span>|<span data-ttu-id="a1fa0-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1fa0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1fa0-111">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1fa0-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="a1fa0-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1fa0-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="a1fa0-113">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="a1fa0-114">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1fa0-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="a1fa0-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1fa0-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="a1fa0-116">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="a1fa0-117">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="a1fa0-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="a1fa0-118">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-118">String</span></span>|<span data-ttu-id="a1fa0-119">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="a1fa0-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="a1fa0-120">属性</span><span class="sxs-lookup"><span data-stu-id="a1fa0-120">Properties</span></span>
|<span data-ttu-id="a1fa0-121">属性</span><span class="sxs-lookup"><span data-stu-id="a1fa0-121">Property</span></span>|<span data-ttu-id="a1fa0-122">类型</span><span class="sxs-lookup"><span data-stu-id="a1fa0-122">Type</span></span>|<span data-ttu-id="a1fa0-123">说明</span><span class="sxs-lookup"><span data-stu-id="a1fa0-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1fa0-124">id</span><span class="sxs-lookup"><span data-stu-id="a1fa0-124">id</span></span>|<span data-ttu-id="a1fa0-125">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-125">String</span></span>|<span data-ttu-id="a1fa0-126">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a1fa0-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a1fa0-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1fa0-127">appleIdentifier</span></span>|<span data-ttu-id="a1fa0-128">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-128">String</span></span>|<span data-ttu-id="a1fa0-129">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a1fa0-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1fa0-130">topicIdentifier</span></span>|<span data-ttu-id="a1fa0-131">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-131">String</span></span>|<span data-ttu-id="a1fa0-132">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-132">Topic Id.</span></span>|
|<span data-ttu-id="a1fa0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1fa0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a1fa0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1fa0-134">DateTimeOffset</span></span>|<span data-ttu-id="a1fa0-135">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a1fa0-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1fa0-136">expirationDateTime</span></span>|<span data-ttu-id="a1fa0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1fa0-137">DateTimeOffset</span></span>|<span data-ttu-id="a1fa0-138">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a1fa0-139">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a1fa0-139">certificateSerialNumber</span></span>|<span data-ttu-id="a1fa0-140">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-140">String</span></span>|<span data-ttu-id="a1fa0-141">证书序列号。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-141">Certificate serial number.</span></span> <span data-ttu-id="a1fa0-142">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-142">This property is read-only.</span></span>|
|<span data-ttu-id="a1fa0-143">证书</span><span class="sxs-lookup"><span data-stu-id="a1fa0-143">certificate</span></span>|<span data-ttu-id="a1fa0-144">String</span><span class="sxs-lookup"><span data-stu-id="a1fa0-144">String</span></span>|<span data-ttu-id="a1fa0-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1fa0-145">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1fa0-146">关系</span><span class="sxs-lookup"><span data-stu-id="a1fa0-146">Relationships</span></span>
<span data-ttu-id="a1fa0-147">无</span><span class="sxs-lookup"><span data-stu-id="a1fa0-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1fa0-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1fa0-148">JSON Representation</span></span>
<span data-ttu-id="a1fa0-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1fa0-149">Here is a JSON representation of the resource.</span></span>
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
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```





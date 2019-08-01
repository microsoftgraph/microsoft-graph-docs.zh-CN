---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c56f78a596d08037ca68a96bf9cc5aca5fbf148
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027501"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="53553-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="53553-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="53553-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53553-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53553-105">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="53553-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="53553-106">方法</span><span class="sxs-lookup"><span data-stu-id="53553-106">Methods</span></span>
|<span data-ttu-id="53553-107">方法</span><span class="sxs-lookup"><span data-stu-id="53553-107">Method</span></span>|<span data-ttu-id="53553-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="53553-108">Return Type</span></span>|<span data-ttu-id="53553-109">说明</span><span class="sxs-lookup"><span data-stu-id="53553-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53553-110">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="53553-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="53553-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="53553-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="53553-112">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53553-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="53553-113">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="53553-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="53553-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="53553-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="53553-115">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53553-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="53553-116">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="53553-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="53553-117">String</span><span class="sxs-lookup"><span data-stu-id="53553-117">String</span></span>|<span data-ttu-id="53553-118">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="53553-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="53553-119">属性</span><span class="sxs-lookup"><span data-stu-id="53553-119">Properties</span></span>
|<span data-ttu-id="53553-120">属性</span><span class="sxs-lookup"><span data-stu-id="53553-120">Property</span></span>|<span data-ttu-id="53553-121">类型</span><span class="sxs-lookup"><span data-stu-id="53553-121">Type</span></span>|<span data-ttu-id="53553-122">说明</span><span class="sxs-lookup"><span data-stu-id="53553-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53553-123">id</span><span class="sxs-lookup"><span data-stu-id="53553-123">id</span></span>|<span data-ttu-id="53553-124">String</span><span class="sxs-lookup"><span data-stu-id="53553-124">String</span></span>|<span data-ttu-id="53553-125">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="53553-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="53553-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="53553-126">appleIdentifier</span></span>|<span data-ttu-id="53553-127">String</span><span class="sxs-lookup"><span data-stu-id="53553-127">String</span></span>|<span data-ttu-id="53553-128">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="53553-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="53553-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="53553-129">topicIdentifier</span></span>|<span data-ttu-id="53553-130">String</span><span class="sxs-lookup"><span data-stu-id="53553-130">String</span></span>|<span data-ttu-id="53553-131">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="53553-131">Topic Id.</span></span>|
|<span data-ttu-id="53553-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53553-132">lastModifiedDateTime</span></span>|<span data-ttu-id="53553-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53553-133">DateTimeOffset</span></span>|<span data-ttu-id="53553-134">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="53553-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="53553-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53553-135">expirationDateTime</span></span>|<span data-ttu-id="53553-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53553-136">DateTimeOffset</span></span>|<span data-ttu-id="53553-137">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="53553-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="53553-138">证书</span><span class="sxs-lookup"><span data-stu-id="53553-138">certificate</span></span>|<span data-ttu-id="53553-139">String</span><span class="sxs-lookup"><span data-stu-id="53553-139">String</span></span>|<span data-ttu-id="53553-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53553-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="53553-141">关系</span><span class="sxs-lookup"><span data-stu-id="53553-141">Relationships</span></span>
<span data-ttu-id="53553-142">无</span><span class="sxs-lookup"><span data-stu-id="53553-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53553-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53553-143">JSON Representation</span></span>
<span data-ttu-id="53553-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53553-144">Here is a JSON representation of the resource.</span></span>
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




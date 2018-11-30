---
title: applePushNotificationCertificate 资源类型
description: Apple 推送通知证书。
ms.openlocfilehash: 7980f615d657b1c79dd09d1f5c06ced58151dbec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008863"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="084c4-103">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="084c4-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="084c4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="084c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="084c4-105">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="084c4-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="084c4-106">方法</span><span class="sxs-lookup"><span data-stu-id="084c4-106">Methods</span></span>
|<span data-ttu-id="084c4-107">方法</span><span class="sxs-lookup"><span data-stu-id="084c4-107">Method</span></span>|<span data-ttu-id="084c4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="084c4-108">Return Type</span></span>|<span data-ttu-id="084c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="084c4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="084c4-110">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="084c4-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="084c4-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="084c4-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="084c4-112">读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="084c4-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="084c4-113">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="084c4-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="084c4-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="084c4-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="084c4-115">更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="084c4-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="084c4-116">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="084c4-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="084c4-117">String</span><span class="sxs-lookup"><span data-stu-id="084c4-117">String</span></span>|<span data-ttu-id="084c4-118">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="084c4-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="084c4-119">属性</span><span class="sxs-lookup"><span data-stu-id="084c4-119">Properties</span></span>
|<span data-ttu-id="084c4-120">属性</span><span class="sxs-lookup"><span data-stu-id="084c4-120">Property</span></span>|<span data-ttu-id="084c4-121">类型</span><span class="sxs-lookup"><span data-stu-id="084c4-121">Type</span></span>|<span data-ttu-id="084c4-122">说明</span><span class="sxs-lookup"><span data-stu-id="084c4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="084c4-123">id</span><span class="sxs-lookup"><span data-stu-id="084c4-123">id</span></span>|<span data-ttu-id="084c4-124">String</span><span class="sxs-lookup"><span data-stu-id="084c4-124">String</span></span>|<span data-ttu-id="084c4-125">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="084c4-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="084c4-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="084c4-126">appleIdentifier</span></span>|<span data-ttu-id="084c4-127">String</span><span class="sxs-lookup"><span data-stu-id="084c4-127">String</span></span>|<span data-ttu-id="084c4-128">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="084c4-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="084c4-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="084c4-129">topicIdentifier</span></span>|<span data-ttu-id="084c4-130">String</span><span class="sxs-lookup"><span data-stu-id="084c4-130">String</span></span>|<span data-ttu-id="084c4-131">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="084c4-131">Topic Id.</span></span>|
|<span data-ttu-id="084c4-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="084c4-132">lastModifiedDateTime</span></span>|<span data-ttu-id="084c4-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="084c4-133">DateTimeOffset</span></span>|<span data-ttu-id="084c4-134">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="084c4-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="084c4-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="084c4-135">expirationDateTime</span></span>|<span data-ttu-id="084c4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="084c4-136">DateTimeOffset</span></span>|<span data-ttu-id="084c4-137">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="084c4-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="084c4-138">certificate</span><span class="sxs-lookup"><span data-stu-id="084c4-138">certificate</span></span>|<span data-ttu-id="084c4-139">String</span><span class="sxs-lookup"><span data-stu-id="084c4-139">String</span></span>|<span data-ttu-id="084c4-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="084c4-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="084c4-141">关系</span><span class="sxs-lookup"><span data-stu-id="084c4-141">Relationships</span></span>
<span data-ttu-id="084c4-142">无</span><span class="sxs-lookup"><span data-stu-id="084c4-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="084c4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="084c4-143">JSON Representation</span></span>
<span data-ttu-id="084c4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="084c4-144">Here is a JSON representation of the resource.</span></span>
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




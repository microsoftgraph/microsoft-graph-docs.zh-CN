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
# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate 资源类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Apple 推送通知证书。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|读取 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性和关系。|
|[更新 applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|更新 [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) 对象的属性。|
|[downloadApplePushNotificationCertificateSigningRequest 函数](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|下载 Apple 推送通知证书签名请求|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|证书的唯一标识符|
|appleIdentifier|String|用于创建 MDM 推送证书的帐户 Apple ID。|
|topicIdentifier|String|主题 ID。|
|lastModifiedDateTime|DateTimeOffset|上次修改 Apple 推送通知证书的日期和时间。|
|expirationDateTime|DateTimeOffset|Apple 推送通知证书的到期日期和时间。|
|证书|String|尚未记录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
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





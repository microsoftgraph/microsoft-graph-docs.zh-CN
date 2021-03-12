---
title: agreementAcceptance 资源类型
description: 表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ac0e6d67e10e7d7b81fc1c5c21e93251f84cab0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722618"
---
# <a name="agreementacceptance-resource-type"></a>agreementAcceptance 资源类型

命名空间：microsoft.graph

表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|agreementFileId|字符串|用户接受的协议文件的标识符。|
|agreementId|字符串|协议的标识符。|
|deviceDisplayName|String|用于显示名称协议的设备的设备组。|
|deviceId|String|用于接受协议的设备的唯一标识符。|
|deviceOSType|字符串|用于接受协议的操作系统。|
|deviceOSVersion|字符串|用于接受协议的设备的操作系统版本。    |
|expirationDateTime|DateTimeOffset|接受的到期日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|字符串| 协议接受的标识符。 只读。|
|recordedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|state|string| 协议接受的状态。 可取值为：`accepted`、`declined`。|
|userDisplayName|String|记录接受时用户的显示名称。|
|userEmail|String|记录接受时用户的电子邮件。|
|userId|字符串|接受该协议的用户的标识符。|
|userPrincipalName|字符串|记录接受时用户的 UPN。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



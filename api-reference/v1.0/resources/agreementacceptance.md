---
title: agreementAcceptance 资源类型
description: 表示由 Azure AD Azure Active Directory (支持的公司可自定义使用条款范围内的用户) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 2df1803b8601635eba163aa3abd46d70ee0a5723
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089968"
---
# <a name="agreementacceptance-resource-type"></a>agreementAcceptance 资源类型

命名空间：microsoft.graph

表示由 Azure AD Azure Active Directory (支持的公司可自定义使用条款范围内的用户) 。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|agreementFileId|String|用户接受的协议文件的标识符。|
|agreementId|String|协议的标识符。|
|deviceDisplayName|String|用于显示名称协议的设备的设备组。|
|deviceId|String|用于接受协议的设备的唯一标识符。|
|deviceOSType|String|用于接受协议的操作系统。|
|deviceOSVersion|String|用于接受协议的设备的操作系统版本。    |
|expirationDateTime|DateTimeOffset|接受的到期日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|String| 协议接受的标识符。 只读。|
|recordedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|state|string| 协议接受的状态。 可取值为：`accepted`、`declined`。|
|userDisplayName|String|记录接受时用户的显示名称。|
|userEmail|String|记录接受时用户的电子邮件。|
|userId|String|接受该协议的用户的标识符。|
|userPrincipalName|String|记录接受时用户的 UPN。|

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



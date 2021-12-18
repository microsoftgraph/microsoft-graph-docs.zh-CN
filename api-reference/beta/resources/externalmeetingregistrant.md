---
title: externalMeetingRegistrant 资源类型
description: 表示已注册联机会议的外部会议注册人。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05c386137ea9e062e223eb7854afc4d13458fe30
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565182"
---
# <a name="externalmeetingregistrant-resource-type"></a>externalMeetingRegistrant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已注册联机会议的外部会议注册人。

继承自 [meetingRegistrantBase](../resources/meetingregistrantbase.md)。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 externalMeetingRegistrants](../api/externalmeetingregistrant-list.md)|[externalMeetingRegistrant](../resources/externalmeetingregistrant.md) 集合|获取 [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) 对象及其属性的列表。|
|[创建 externalMeetingRegistrant](../api/externalmeetingregistrant-post.md)|[externalMeetingRegistrant](../resources/externalmeetingregistrant.md)|读取 [externalMeetingRegistrant 对象的属性和](../resources/externalmeetingregistrant.md) 关系。|
|[删除 externalMeetingRegistrant](../api/externalmeetingregistrant-delete.md)|无|删除 [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) 对象。|

## <a name="properties"></a>属性

| 属性   | 类型   | 说明                                                                  |
|:-----------|:-------|:-----------------------------------------------------------------------------|
| id         | String | 外部注册系统中注册者的唯一标识符。 继承自 [meetingRegistrantBase](../resources/meetingregistrantbase.md)。 |
| joinWebUrl | String | 注册人加入会议的唯一 Web URL。 继承自 [meetingRegistrantBase](../resources/meetingregistrantbase.md)。 只读。          |
| tenantId   | 字符串 | 此注册表项的租户 ID（如果Azure Active Directory）。               |
| userId     | 字符串 | 此注册表项的用户 ID（如果Azure Active Directory）。                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "baseType": "microsoft.graph.meetingRegistrantBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "userId": "String",
  "tenantId": "String"
}
```

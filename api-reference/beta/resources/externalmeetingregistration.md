---
title: externalMeetingRegistration 资源类型
description: 包含有关外部会议注册的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: af59114df32f24c36c1cd8d75e344162ac6e0d88
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565178"
---
# <a name="externalmeetingregistration-resource-type"></a>externalMeetingRegistration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示联机会议的外部注册详细信息。

继承自 [meetingRegistrationBase](meetingregistrationbase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalMeetingRegistration](../api/externalmeetingregistration-post.md)|[externalMeetingRegistration](externalmeetingregistration.md)|创建新的 [externalMeetingRegistration](externalmeetingregistration.md) 对象。|
|[获取 externalMeetingRegistration](../api/externalmeetingregistration-get.md)|[externalMeetingRegistration](externalmeetingregistration.md)|读取 [externalMeetingRegistration 对象的属性和](externalmeetingregistration.md) 关系。|
|[删除 externalMeetingRegistration](../api/externalmeetingregistration-delete.md)|无|删除 [externalMeetingRegistration](externalmeetingregistration.md) 对象。|

## <a name="properties"></a>属性

| 属性          | 类型                                       | 说明                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | 指定可注册会议的人。 继承自 [meetingRegistrationBase](meetingregistrationbase.md)。 |

### <a name="meetingaudience-values"></a>meetingAudience 值

| 值              | 说明                                                            |
|--------------------|------------------------------------------------------------------------|
| everyone           | 每个人都可以注册会议。                                 |
| 组织       | 组织者组织中的每个人都可以注册会议。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。                      |

## <a name="relationships"></a>关系

| 关系 | 类型                                                                 | 说明                        |
|:-------------|:---------------------------------------------------------------------|:-----------------------------------|
| registrants  | [externalMeetingRegistrant](externalmeetingregistrant.md) 集合 | 联机会议注册人。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistration",
  "baseType": "microsoft.graph.meetingRegistrationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.externalMeetingRegistrant" }]
}
```

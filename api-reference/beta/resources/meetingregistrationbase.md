---
title: meetingRegistrationBase 资源类型
description: 包含有关基本会议注册的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 01bdfeaa222464c7e7b44bf5f92482b2b1c3d4e0
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565173"
---
# <a name="meetingregistrationbase-resource-type"></a>meetingRegistrationBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示联机会议的基本注册详细信息。

[meetingRegistration 和](meetingregistration.md) [externalMeetingRegistration 的基本类型](externalmeetingregistration.md)。

> [!TIP]
> 这是抽象类型，不能直接使用。 请改为使用派生类型[meetingRegistration](meetingregistration.md)或[externalMeetingRegistration。](externalmeetingregistration.md)

## <a name="properties"></a>属性

| 属性          | 类型                                       | 说明                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | 指定可注册会议的人。 |

### <a name="meetingaudience-values"></a>meetingAudience 值

| 值              | 说明                                                            |
|--------------------|------------------------------------------------------------------------|
| everyone           | 每个人都可以注册会议。                                 |
| 组织       | 组织者组织中的每个人都可以注册会议。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。                      |

## <a name="relationships"></a>关系

| 关系 | 类型                                                         | 说明                        |
|:-------------|:-------------------------------------------------------------|:-----------------------------------|
| registrants  | [meetingRegistrantBase](meetingregistrantbase.md) 集合 | 联机会议注册人。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrationBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrationBase",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrantBase" }]
}
```

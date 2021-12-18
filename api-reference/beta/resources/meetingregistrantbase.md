---
title: meetingRegistrantBase 资源类型
description: 表示已注册联机会议的基本会议注册人。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c17ccf2cb3b34b9b139726b727cd84148b6bc9a8
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565177"
---
# <a name="meetingregistrantbase-resource-type"></a>meetingRegistrantBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已注册联机会议的基本会议注册人。

[meetingRegistrant 和](meetingregistrant.md) [externalMeetingRegistrant 的基类型](externalmeetingregistrant.md)。

> [!TIP]
> 这是抽象类型，不能直接使用。 请改为使用派生类型[meetingRegistrant](meetingregistrant.md)或[externalMeetingRegistrant。](externalmeetingregistrant.md)

## <a name="properties"></a>属性

| 属性   | 类型   | 说明                                                         |
|:-----------|:-------|:--------------------------------------------------------------------|
| id         | String | 注册表的唯一标识符。 只读。                 |
| joinWebUrl | String | 注册人加入会议的唯一 Web URL。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrantBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrantBase",
  "id": "String (identifier)",
  "joinWebUrl": "String"
}
```

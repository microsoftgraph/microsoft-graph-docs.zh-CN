---
title: joinMeetingIdSettings 资源类型
description: 指定 joinMeetingId、会议密码和密码要求。
author: yuyaolian-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fc954abe7c265c864587fdc5c2c6150c78374970
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645616"
---
# <a name="joinmeetingidsettings-resource-type"></a>joinMeetingIdSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定 **joinMeetingId**、会议密码以及联机会议的密码要求。

## <a name="properties"></a>属性

| 属性            | 类型      | 说明                                   |
|:--------------------|:----------|:----------------------------------------------|
| isPasscodeRequired  | Boolean   | 指示在使用 **joinMeetingId** 时是否需要密码才能加入会议。 可选。 |
| joinMeetingId       | String    | 用于加入会议的会议 ID。 可选。 只读。 |
| 密码            | String    | 要加入会议的密码。  可选。 只读。 |
## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.joinMeetingIdSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.joinMeetingIdSettings",
  "isPasscodeRequired": "Boolean",
  "joinMeetingId": "String",
  "passcode": "String"
}
```

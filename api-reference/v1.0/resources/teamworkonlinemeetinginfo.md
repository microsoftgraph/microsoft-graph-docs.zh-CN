---
title: teamworkOnlineMeetingInfo 资源类型
description: 表示有关 Microsoft Teams 中的联机会议的详细信息。
author: jecha
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac6dab85a12cdb339bb6527a6c1c436285c1ea75
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443260"
---
# <a name="teamworkonlinemeetinginfo-resource-type"></a>teamworkOnlineMeetingInfo 资源类型

命名空间：microsoft.graph

表示有关 Microsoft Teams 中的联机会议的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|calendarEventId|String|与会议关联的日历事件的标识符。|
|joinWebUrl|String|用户单击以加入或唯一标识会议 URL。|
|组织者|[teamworkUserIdentity](teamworkuseridentity.md)|会议的组织者。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
}
-->
``` json
{
  "calendarEventId": "string",
  "joinWebUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.teamworkUserIdentity"}
}
```

## <a name="see-also"></a>另请参阅
- [聊天](chat.md)

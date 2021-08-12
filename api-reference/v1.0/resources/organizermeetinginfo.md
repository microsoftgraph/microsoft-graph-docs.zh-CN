---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fc97e94b2657273a55798528991762e43ec98023ba3e861f51a0e03d3d27f13f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178127"
---
# <a name="organizermeetinginfo-resource-type"></a>organizerMeetingInfo 资源类型

命名空间：microsoft.graph

包含有关会议组织者的详细信息。 

若要加入现有会议，您必须提供 organizerMeetingInfo 和 [chatInfo](./chatinfo.md) 资源类型的组合，或者 [提供 tokenMeetingInfo](./tokenmeetinginfo.md) 资源类型本身的组合。

## <a name="properties"></a>属性

| 属性                     | 类型                          | 说明                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| organizer － 组织者                    | [identitySet](identityset.md) | 组织者Azure Active Directory标识。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


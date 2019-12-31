---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e7750e282801a938fd42c01717cc7bbbedcf95a3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913679"
---
# <a name="organizermeetinginfo-resource-type"></a>organizerMeetingInfo 资源类型

包含有关会议组织者的详细信息。 

若要加入现有会议，必须提供 organizerMeetingInfo 和[chatInfo](./chatinfo.md)资源类型或[tokenMeetingInfo](./tokenmeetinginfo.md)资源类型的组合。

## <a name="properties"></a>属性

| 属性                     | 类型                          | 说明                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| organizer － 组织者                    | [identitySet](identityset.md) | 组织者 Azure Active Directory 标识。  |

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

---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d3b1f37e6ac5f33d6d59988054d5abfedf5e68e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066283"
---
# <a name="organizermeetinginfo-resource-type"></a>organizerMeetingInfo 资源类型

命名空间：microsoft.graph

包含有关会议组织者的详细信息。 

若要加入现有会议，必须提供 organizerMeetingInfo 和 [chatInfo](./chatinfo.md) 资源类型或 [tokenMeetingInfo](./tokenmeetinginfo.md) 资源类型的组合。

## <a name="properties"></a>属性

| 属性                     | 类型                          | 说明                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| 组织者                    | [identitySet](identityset.md) | 组织者 Azure Active Directory 标识。  |

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


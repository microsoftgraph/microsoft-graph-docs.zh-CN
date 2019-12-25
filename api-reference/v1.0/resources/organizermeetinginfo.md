---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab1d907365e40b70a8d85a845c9e8ec0366183af
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871066"
---
# <a name="organizermeetinginfo-resource-type"></a>organizerMeetingInfo 资源类型

包含有关会议组织者的详细信息。 

若要加入现有会议，必须提供 organizerMeetingInfo 和[chatInfo](./chatinfo.md)资源类型或[tokenMeetingInfo](./tokenmeetinginfo.md)资源类型的组合。

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

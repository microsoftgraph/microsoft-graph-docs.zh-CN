---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b3d8671c33a0040fde8671a2d97b67dae0e94b28
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913581"
---
# <a name="participantinfo-resource-type"></a>participantInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关参与者标识的其他属性

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | String                        | 呼叫开始时参与者最佳估计物理位置的 ISO 3166-1 Alpha-2 国家/地区代码。 只读。                             |
| endpointType   | String                        | 参与者正在使用的终结点的类型。 可能的值包括`default`： `skypeForBusiness`、或`skypeForBusinessVoipPhone`。 只读。              |
| 窃取       | [identitySet](identityset.md) | 与此参与者关联的[了解 identityset](identityset.md) 。 只读。                                                                             |
| languageId     | String                        | 语言区域性字符串。 只读。                                                                                                                    |
| 范围         | String                        | 参与者的家乡区域。 它可以是国家/地区、一个洲或更大的地理区域。 这不会根据参与者的当前物理位置而变化，这与 countryCode 不同。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

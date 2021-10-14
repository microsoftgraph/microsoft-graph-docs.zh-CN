---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f6c759ba3936d500b34566ac894895ce7b0f7ff7
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289852"
---
# <a name="participantinfo-resource-type"></a>participantInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关参与者标识的其他属性

## <a name="properties"></a>属性

| 属性         | 类型                            | 说明                                                                                                                                                                                                      |
| :--------------- | :------------------------------ | :-----------------------------------------------------------------------------------------------------------------------------------------------------------                                                     |
| countryCode      | String                          | 呼叫开始时参与者的最佳估计物理位置的 ISO 3166-1 Alpha-2 国家/地区代码。 只读。                                                                                   |
| endpointType     | 字符串                          | 参与者使用的终结点类型。 可能的值为： `default`、 `skypeForBusiness`或 `skypeForBusinessVoipPhone`。 只读。                                                                    |
| identity         | [identitySet](identityset.md)   | 与此[参与者关联的 identitySet。](identityset.md) 只读。                                                                                                                                   |
| languageId       | 字符串                          | 语言区域性字符串。 只读。                                                                                                                                                                          |
| region           | 字符串                          | 参与者的主页区域。 它可以是国家/地区、洲或较大的地理区域。 这与 countryCode 不同，这不会基于参与者的当前物理位置而更改。 只读。 |
| platformId       | 字符串                          | 参与者的客户端平台 ID。 只读。    |
| participantId    | 字符串                          | 参与者的参与者 ID。 只读。    |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region",
    "platformId",
    "participantId"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String",
  "platformId": "String",
  "participantId": "String"
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



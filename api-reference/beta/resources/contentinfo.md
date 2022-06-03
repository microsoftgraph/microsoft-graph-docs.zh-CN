---
title: contentInfo 资源类型
description: 表示要标记的某些信息的当前状态。
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7dc6c99e1c4c19564e17c406beca02971071c671
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884172"
---
# <a name="contentinfo-resource-type"></a>contentInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要标记的某些信息的当前状态。 **contentInfo** 将传递到 [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md) 和 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) API，以向 API 描述信息的当前状态。 此 **contentInfo** 详细信息驱动在应用、更新或删除标签时应添加或删除哪些元数据、内容标记和保护的结果。 

## <a name="properties"></a>属性

| 属性   | 类型                                       | 说明                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| format     | String                                     | 可取值为：`default`、`email`。                                                                                        |
| 标识符 | String                                     | 用于 Azure 信息保护分析的标识符。                                                                     |
| 元   | [keyValuePair](keyvaluepair.md) 集合 | 现有的 Microsoft Purview 信息保护元数据作为键/值对传递，其中密钥为MSIP_Label_GUID_PropName。 |
| state      | String                                     | 可取值为：`rest`、`motion`、`use`。                                                                                   |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


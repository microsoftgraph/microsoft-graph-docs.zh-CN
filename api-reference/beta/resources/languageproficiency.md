---
title: languageProficiency 资源类型
description: languageProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3a022d9c255bbfee03ef7f1fec891bc0fa757480
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950456"
---
# <a name="languageproficiency-resource-type"></a>languageProficiency 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户已添加到其[配置文件](profile.md)中的语言的详细信息。

继承自[itemFacet](itemFacet.md)。

## <a name="methods"></a>方法

| 方法                                                       | 返回类型                                   | 说明                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [获取 languageProficiency](../api/languageproficiency-get.md) | [languageProficiency](languageproficiency.md) | 读取**languageProficiency**对象的属性和关系。 |
| [更新 languageProficiency](../api/languageproficiency-update.md)               | [languageProficiency](languageproficiency.md) | 更新**languageProficiency**对象。                               |
| [删除 languageProficiency](../api/languageproficiency-delete.md)               | 无                                          | 删除**languageProficiency**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String       | 包含语言的长格式名称。                                                                                                   |
|水平   |string       | 可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。|
|tag           |String       | 包含四个字符的语言的 BCP47 名称（en-us，无 NB，en-us）。                                                                                  |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

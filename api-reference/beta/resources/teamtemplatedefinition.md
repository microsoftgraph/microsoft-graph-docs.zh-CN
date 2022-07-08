---
title: teamTemplateDefinition
description: 具有特定结构和配置的团队的团队模板定义的通用表示形式。
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 9df396be7eca713cd407c253af8285528e6587f8
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690101"
---
# <a name="teamtemplatedefinition-resource-type"></a>teamTemplateDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

具有特定结构和配置的团队的团队模板定义的通用表示形式。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 teamTemplateDefinition](../api/teamtemplatedefinition-get.md)|[teamTemplateDefinition](../resources/teamtemplatedefinition.md)|读取 [teamTemplateDefinition](../resources/teamtemplatedefinition.md) 对象的属性和关系。|
| [列出 teamTemplateDefinitions](../api/teamtemplate-list-definitions.md) | [teamTemplateDefinition](../resources/teamtemplatedefinition.md) 集合 | 列出与 **teamTemplate** 关联的 **teamTemplateDefinition** 对象。  |
| [获取 teamDefinition](../api/teamtemplatedefinition-get-teamdefinition.md) | [团队](../resources/team.md) | 读取 **teamTemplateDefinition** 对象的 **团队** 的属性 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|观众|teamTemplateAudience|介绍团队模板可用的受众。 可能的值包括 `organization`、`user`、`public`、`unknownFutureValue`。|
|类别|String collection|团队模板的分配类别。|
|说明|String|团队模板的简要说明，因为它将显示在 Microsoft Teams 中的用户中。|
|displayName|String|团队模板的用户定义名称。|
|iconUrl|String|团队模板的图标 URL。|
|id|String|团队模板的`templateId` +  + `audience``locale`编码 64。 继承自 [entity](../resources/entity.md)。|
|languageTag|字符串|模板可用的语言。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改团队模板的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改团队模板的日期时间。|
|parentTemplateId|字符串|团队 `templateId` 模板|
|publisherName|String|发布团队模板的组织。|
|shortDescription|String|团队模板的简短说明，因为它将显示在 Microsoft Teams 中的用户中。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|teamDefinition|[团队](../resources/team.md)|[通道](../resources/channel.md)对象的集合。 频道表示团队内部的某个主题，因此是讨论的逻辑隔离。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamtemplatedefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamTemplateDefinition",
  "id": "String (identifier)",
  "parentTemplateId": "String",
  "displayName": "String",
  "languageTag": "String",
  "audience": "String",
  "description": "String",
  "shortDescription": "String",
  "iconUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "publisherName": "String",
  "categories": [
    "String"
  ]
}
```
## <a name="see-also"></a>另请参阅

- [团队](team.md)
- [teamsTemplate](teamsTemplate.md)

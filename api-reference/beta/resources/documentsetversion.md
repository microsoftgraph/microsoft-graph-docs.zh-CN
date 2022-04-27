---
title: documentSetVersion 资源类型
description: 表示列表中文档集项的版本。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c86cad9d0e5fe251c3d67145f56c9de2578b22c3
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061178"
---
# <a name="documentsetversion-resource-type"></a>documentSetVersion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示列表中文档集项的版本。

继承自 [listItemVersion](../resources/listitemversion.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 documentSetVersions](../api/listitem-list-documentsetversions.md)|[documentSetVersion](../resources/documentsetversion.md) 集合|从 [documentSetVersions](../resources/documentsetversion.md) 导航属性获取 **documentSetVersion 资源** 。|
|[创建 documentSetVersion](../api/listitem-post-documentsetversions.md)|[documentSetVersion](../resources/documentsetversion.md)|创建新的 [documentSetVersion](../resources/documentsetversion.md) 对象。|
|[获取 documentSetVersion](../api/documentsetversion-get.md)|[documentSetVersion](../resources/documentsetversion.md)|读取 [documentSetVersion](../resources/documentsetversion.md) 对象的属性和关系。|
|[删除 documentSetVersion](../api/documentsetversion-delete.md)|无|删除 [documentSetVersion](../resources/documentsetversion.md) 对象。|
|[恢复](../api/documentsetversion-restore.md)|[documentSetVersion](../resources/documentsetversion.md)|还原 [documentSetVersion](../resources/documentsetversion.md)。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| comment | string | 对捕获的版本进行注释。|
| createdBy   | [identitySet](../resources/identityset.md) | 捕获版本的用户。|
| createdDateTime     | dateTime | 创建此版本的日期和时间。|
| id                  | string                                               | 版本 ID。 只读。 继承自 [listItemVersion](../resources/listitemversion.md)。|
| items     | [documentSetVersionItem](../resources/documentsetversionitem.md) 集合 | 作为此版本的一部分捕获的文档集中的项。|
| lastModifiedBy       | [identitySet](../resources/identityset.md)           | 上次修改版本的用户的标识。 只读。 继承自 [listItemVersion](../resources/listitemversion.md)。|
| lastModifiedDateTime | [dateTimeOffset](../resources/timestamp.md)          | 上次修改版本的日期和时间。 只读。 继承自 [listItemVersion](../resources/listitemversion.md)。     |
| 发表            | [publicationFacet](../resources/publicationfacet.md) | 指示此特定版本的发布状态。 只读。 继承自 [listItemVersion](../resources/listitemversion.md)。| 
| shouldCaptureMinorVersion | 布尔  | 如果 `true`还捕获了次要版本的项目，则仅捕获主要版本。 默认值为 `false`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
| fields        | [fieldValueSet](../resources/fieldvalueset.md) | 此版本列表项的字段和值集合。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentSetVersion",
  "baseType": "microsoft.graph.listItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersion",
  "comment": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "items": [
    {
      "@odata.type": "microsoft.graph.documentSetVersionItem"
    }
  ],
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "shouldCaptureMinorVersion": "Boolean"
}
```


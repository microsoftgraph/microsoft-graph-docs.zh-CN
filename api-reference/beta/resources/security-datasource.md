---
title: dataSource 资源类型
description: dataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d95cdd3dd8f66c2c4de67c8c469281989e839f93
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945321"
---
# <a name="datasource-resource-type"></a>dataSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

dataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。

## <a name="methods"></a>方法

无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **dataSource** 的用户。|
|createdDateTime|DateTimeOffset|**创建 dataSource** 的日期和时间。|
|displayName|String|**dataSource** 的显示名称。 这将是 SharePoint 网站的名称。|
|id|String| **dataSource** 的 ID。 这不是实际网站的 ID。|
|holdStatus|字符串|**dataSource** 的保留状态。可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|
## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


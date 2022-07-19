---
title: siteSource 资源类型
description: 与保管人关联的站点的容器。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0dd23c703ef63c11da357ac6db0d0dfdc73a5212
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837532"
---
# <a name="sitesource-resource-type"></a>siteSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
与保管人关联的站点的容器。

继承自 [dataSource](../resources/security-datasource.md)。


## <a name="methods"></a>方法
无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **siteSource** 的用户。|
|createdDateTime|DateTimeOffset|**网站源** 的创建日期和时间。|
|displayName|String|**siteSource** 的显示名称。 这将是 SharePoint 网站的名称。|
|id|String| **siteSource** 的 ID。 |
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|**siteSource** 的保留状态。 可能的值包括 `notApplied`、`applied`、`applying`、`removing`、`partial`。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|网站|[site](../resources/site.md)|与 **siteSource** 关联的 SharePoint 网站。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


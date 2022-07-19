---
title: unifiedGroupSource 资源类型
description: 保管人的组的容器。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a6b8b05c3f57e4903b66aa7de95e8b4d94849d71
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837805"
---
# <a name="unifiedgroupsource-resource-type"></a>unifiedGroupSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

保管人的组的容器。

继承自 [dataSource](../resources/security-datasource.md)。

## <a name="methods"></a>方法
无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **unifiedGroupSource** 的用户。|
|createdDateTime|DateTimeOffset|创建 **unifiedGroupSource** 的日期和时间。|
|displayName|String|统一组的显示名称，即组的名称。|
|id|String|**unifiedGroupSource** 的 ID。 这不是实际组的 ID。|
|includedSources|microsoft.graph.security.sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|**unifiedGroupSource** 的保留状态。 可能的值包括 `notApplied`、`applied`、`applying`、`removing`、`partial`。|

### <a name="sourcetype-values"></a>sourceType 值
|成员|说明|
|:----|-----------|
| 邮箱 | 表示邮箱。|
| 网站 | 表示 SharePoint 网站。|


## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|组|[group](../resources/group.md)|表示组。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.unifiedGroupSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.unifiedGroupSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "includedSources": "String"
}
```


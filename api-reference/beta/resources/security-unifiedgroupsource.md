---
title: unifiedGroupSource 资源类型
description: 保管人的组的容器。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3e544a4b6d00bb59b5879fc13376fd94a5bba169
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945147"
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
|displayName|String|统一组的显示名称 - 这是组的名称。|
|id|字符串|**unifiedGroupSource** 的 ID。 这不是实际组的 ID。|
|includedSources|String|指定此组中包含的源。 可取值为：`mailbox`、`site`。|
|holdStatus|字符串|**unifiedGroupSource** 的保留状态。可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|组|[组](../resources/group.md)|表示组。|

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


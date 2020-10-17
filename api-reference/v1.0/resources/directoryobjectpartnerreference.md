---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的 directory 对象的引用。 继承自 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 39a3077862727f4d8457a6d0105f03296ba67950
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582154"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference 资源类型

命名空间：microsoft.graph

表示对合作伙伴组织中的目录对象的引用。 继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|字符串| 返回的对象的说明。 只读。 |
|displayName|字符串| 返回的目录对象的名称，如 group 或 application。 只读。 |
|externalPartnerTenantId|Guid| 合作伙伴租户的租户标识符。 只读。 |
|id|字符串| 资源的唯一标识符。 继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。 只读。 |
|objectType|String| 合作伙伴租户中被引用对象的类型。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>另请参阅

- [获取 ID 列表中的目录对象](../api/directoryobject-getbyids.md)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

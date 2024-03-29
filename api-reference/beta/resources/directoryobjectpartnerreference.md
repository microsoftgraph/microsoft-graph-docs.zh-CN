---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0b8825a7bd20e7e76aa3825cf29e8b7246e3ad8a
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855075"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对合作伙伴组织中目录对象的引用。 继承自 [directoryObject](directoryobject.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|String| 返回的对象的说明。 只读。 |
|displayName|字符串| 要返回的目录对象的名称，如组或应用程序。 只读。 |
|externalPartnerTenantId|GUID| 合作伙伴租户的租户标识符。 只读。 |
|id|String| 资源的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 只读。 |
|objectType|String| 合作伙伴租户中引用的对象的类型。 只读。 |

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

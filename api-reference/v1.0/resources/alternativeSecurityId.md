---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
ms.localizationpriority: medium
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9ef21767ee3d38dbba4ad661c0529e2f01a10ba9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036772"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId 资源类型

命名空间：microsoft.graph

仅供内部使用。 将来将弃用此复杂类型。

## <a name="json-representation"></a>JSON 表示形式

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>属性
| 属性         | 类型       | 说明
|:-----------------|:-----------|:---------------------
| 类型             | Int32      | 仅供内部使用
| identityProvider | string     | 仅供内部使用
| 注册表项              | Edm.Binary | 仅供内部使用


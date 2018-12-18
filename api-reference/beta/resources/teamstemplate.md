---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
author: nkramer
ms.openlocfilehash: b4e32448f864048fdcb54dc001b21b262df2bba3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327711"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

工作组模板是在 Microsoft 团队中创建[团队](../resources/team.md)蓝图。 模板指定在使用模板创建新团队结构、 设置和偶数应设置的内容。 Microsoft 提供了一套基本模板，客户可以节省自己的自定义模板。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | 字符串   | 模板的唯一标识符。 不能为 null。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>另请参阅

- [团队](team.md)


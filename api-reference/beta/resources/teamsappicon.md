---
title: teamsAppIcon 资源类型
description: 与 Microsoft Teams 上的应用相关联的图标。
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882652"
---
# <a name="teamsappicon-resource-type"></a>teamsAppIcon 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与 [teamsApp](teamsapp.md)相关联的图标。

## <a name="methods"></a>方法

| 方法                                            | 返回类型                                       | 说明                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [获取图标](../api/teamsappicon-get.md)     | [teamsAppIcon](teamsappicon.md)                   | 获取与 Teams 应用的特定版本相关联的图标。 |
| [获取托管内容](../api/teamworkhostedcontent-get.md) | [teamworkHostedContent](teamworkhostedcontent.md) | 获取托管内容 (及其字节数) 图标的字节数。                |

## <a name="properties"></a>属性

| 属性      | 类型                        | 说明                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| id            | string                      | 应用图标的唯一 ID。                                                          |
| webUrl        | string                      | 可用于下载图像的 Web URL。                                 |

## <a name="relationships"></a>关系

| 关系  | 类型                                              | 说明                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| hostedContent | [teamworkHostedContent](teamworkhostedcontent.md) | 如果图标托管在 Teams 基础结构中，则应用图标的内容。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)

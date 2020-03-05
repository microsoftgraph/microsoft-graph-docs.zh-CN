---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 207fee7f889c4369862918943371e2d629c8fab9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502170"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在 CSV 文件为输入源时设置学校数据同步配置文件。  

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **操作** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 要应用于同步配置文件的可选自定义项。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```

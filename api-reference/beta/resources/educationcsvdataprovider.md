---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60377b1761bcb5c672ae42f3067bb20d41325e9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095532"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在 CSV 文件为输入源时设置学校数据同步配置文件。

派生自 [educationSynchronizationDataProvider]。

## <a name="properties"></a>属性

| 属性       | 类型                                     | 说明                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| 操作 | [educationSynchronizationCustomizations] | 要应用于同步配置文件的可选自定义项。 |

[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

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
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```



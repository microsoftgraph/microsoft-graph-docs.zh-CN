---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33cb0268eeb8c6d6b896dfb8ab02f7bb59b00e98
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434982"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在 CSV 文件为输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider]。

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

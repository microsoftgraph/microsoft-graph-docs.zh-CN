---
title: educationCsvDataProvider 资源类型
description: '用于输入的源 CSV 文件时设置学校数据同步配置文件。  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041862"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

用于输入的源 CSV 文件时设置学校数据同步配置文件。  

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **自定义项** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 可选自定义项应用于同步配置文件。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```

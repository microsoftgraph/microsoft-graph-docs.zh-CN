---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 51563255c11406c26cfa3b02b7b7bb868ed935c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415654"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 

>**注意：****SynchronizationStartDate**属性仅适用于**StudentEnrollment**实体。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | 字符串集合 |  要同步的属性名称的集合。如果设置为 null，所有属性将都为同步。       |
| **synchronizationStartDate** | 日期/时间 |  同步的开始日期。 此值应设置为未来日期。 如果配置文件安装完成后，将会同步设置为 null，资源。 **注意：** 这仅适用于**StudentEnrollment**属性。      |
|**isSyncDeferred** |Boolean | 指示是否对父实体的同步推迟到以后。 |
| **allowDisplayNameUpdate** | Boolean |  指示是否可以通过同步来覆盖资源的显示名称。         |


## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```

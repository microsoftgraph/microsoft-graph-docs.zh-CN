---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体的学校数据配置文件同步的设置。 自定义项可应用于要同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c3f704339dbf2acbe7cb78e1899c5f209f50f21e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055589"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于自定义资源实体的学校数据配置文件同步的设置。 自定义项可应用于要同步的所有实体。

## <a name="properties"></a>属性

| 属性                 | 类型              | 说明                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| optionalPropertiesToSync | String 集合 | 要同步的属性名称的集合。如果设置为 null，则将同步所有属性。 **不适用于学生注册或教师名册**                                                            |
| synchronizationStartDate | 日期时间          | 同步应开始的日期。 此值应设置为将来日期。 如果设置为 null，则在配置文件设置完成时将同步资源。 **仅适用于学生注册** |
| isSyncDeferred           | Boolean           | 指示是否将父实体的同步延迟到更高的日期。                                                                                                                                    |
| allowDisplayNameUpdate   | Boolean           | 指示是否可由同步覆盖资源的显示名称。                                                                                                                                     |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```



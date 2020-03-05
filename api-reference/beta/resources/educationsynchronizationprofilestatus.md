---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500028"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。 

> **注意：** 由于后台同步处理的异步特性，对**educationSynchronizationProfileStatus**的更新可能会延迟。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [获取同步状态](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 返回特定同步配置文件的状态。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | 同步的状态。可能的值为`paused`： `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`、。 |
| **lastSynchronizationDateTime** | DateTimeOffset | 表示在目录中观察到的最新更改的时间。  |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```

---
title: educationSynchronizationProfileStatus 资源类型
description: '代表学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d16619b0cf1e2c09358cf585b896b0c7c7d4f318
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928925"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。 

> **注意：** 更新**educationSynchronizationProfileStatus**可能由于后台同步处理的异步特性延迟。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [要获取同步的状态](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 返回一个特定的同步配置文件的状态。 |

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **status** | string | 同步状态。可能的值为： `paused`， `inProgress`， `success`， `error`， `quarantined`， `validationError`。 |
| **lastSynchronizationDateTime** | DateTimeOffset | 表示当观察的目录中最新更改的时间。  |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```

---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 55636a78cd904c6992de0cf48ab333ccef8bb84a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534191"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校数据同步配置文件 的 [同步状态](educationsynchronizationprofile.md)。

> **注意：** 由于后台同步处理的异步特性 **，educationSynchronizationProfileStatus** 的更新可能会延迟。

## <a name="methods"></a>方法

| 方法                                                                      | 返回类型                               | 说明                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [获取同步状态](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 返回特定同步配置文件的状态。 |

## <a name="properties"></a>属性

| 属性                    | 类型                           | 说明                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| id                          | String                         | 资源的唯一标识符。  (只读)                                                                       |
| status                      | educationSynchronizationStatus | 同步的状态。可能的值是 `paused` `inProgress` `success` ：、、、、、、、。 `error` `quarantined` `validationError` `extracting` *`validating`* |
| lastSynchronizationDateTime | DateTimeOffset                 | 表示最近成功同步的时间。                                        |
| lastActivityDateTime | DateTimeOffset                 | 表示在配置文件中观察到最新更改的时间。                                        |
| errorCount | Int                 | 同步期间的错误数。                                        |
| statusMessage | String                 | 当前配置文件的同步阶段的状态消息。                                        |

"正在提取"和"正在验证"状态仅返回准备处理新枚举成员的应用程序。 选择加入通过设置 HTTP 首选请求标头完成 `Prefer: include-unknown-enum-members` ：。 请参阅有关： [可发展枚举的更多信息](/graph/best-practices-concept#evolvable-enums)。


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
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset",
  "lastActivityDateTime": "DateTimeOffset",
  "errorCount": "Int",
  "statusMessage": "String"
}
```

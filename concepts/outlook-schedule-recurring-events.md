---
title: 在 Outlook 中将重复约会安排为定期事件
description: 重复发生的事件是 Outlook 日历的一个重要部分。无论是与经理每周进行的一对一会议，还是每月第二个星期二的部门评审会议，定期规则只需要创建一次事件，然后让服务器填充系列中的其他内容，从而使过程变得简单。
author: harini84
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 29aeef98cbc0e9d33df26a0c54bb568317ebb790
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071782"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a>在 Outlook 中将重复约会安排为定期事件

重复发生的事件是 Outlook 日历的一个重要部分。无论是与经理每周进行的一对一会议，还是每月第二个星期二的部门评审会议，定期规则只需要创建一次事件，然后让服务器填充系列中的其他内容，从而使过程变得简单。

使定期事件得以“扩展”为单个事件的关键信息点在于定期规则。 此规则同时指定事件重复的频率和持续时间。 Outlook REST API 在 [事件资源](/graph/api/resources/event?view=graph-rest-1.0)的 **重复周期** 属性中模拟定期规则。 

每个重复周期由两部分组成：定期模式（频率）和定期范围（持续时间）。

## <a name="recurrence-patterns"></a>定期模式

重复的第一部分是模式。 它指定事件重复的频率。 例如，一个事件可以“每 3 天”、“每周四”或“每年的 7 月 22 日”重复一次。 在 API 中，模式由 [recurrencePattern 资源](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)表示。

**recurrencePattern** 的特定字段是必需、可选还是忽略取决于模式的类型。

> **注意**：即使将字段忽略，仍需验证该字段。 如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。

让我们来看看每个可能的模式类型。

### <a name="daily"></a>每天

每天定期模式会导致事件基于每次事件之间的天数重复。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **interval** | 必需 | 指定每次事件之间的天数。 |
| **type** | 必需 | 必须设置为 `daily`。 |

#### <a name="examples"></a>示例

- 每天重复此事件

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- 每三天重复此事件

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a>每周

每周定期模式使事件基于每组事件之间的周数，在每周的同一天或几天重复。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必需 | 指定事件发生在每周的哪一天/哪几天。 |
| **firstDayOfWeek** | 可选 | 指定将哪一天视为一周的第一天。 默认值为：`Sunday`。 |
| **interval** | 必需 | 指定每组事件之间的周数。 |
| **type** | 必需 | 必须设置为 `weekly`。 |

#### <a name="examples"></a>示例

- 每周四重复此事件

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- 每隔一个周一和周二重复此事件

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a>绝对每月

绝对每月模式使事件在每个月的同一天（例如，15日）重复，它基于每次事件之间的月数。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **dayOfMonth** | 必需 | 指定事件发生在每月的哪一天。 |
| **interval** | 必需 | 指定每次事件之间的月数。 |
| **type** | 必需 | 必须设置为 `absoluteMonthly`。 |

#### <a name="examples"></a>示例

- 在每月的 15 号重复此事件。

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- 按季度（每 3 个月）在 7 号重复此事件

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a>相对每月

相对每月模式使事件基于每次事件之间的月数，在每个月同一相对位置中每周的同一天重复。例如，“每个月的第二个星期三”。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必需 | 指定该事件可以在一周中的哪一天发生。相对每月事件每月仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。 |
| **index** | 可选 | 指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。 可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。 默认值为：`first`。 |
| **interval** | 必需 | 指定每次事件之间的月数。 |
| **type** | 必需 | 必须设置为 `relativeMonthly`。 |

#### <a name="examples"></a>示例

- 在每月的第二个星期三重复此事件

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- 在每月的第一个星期四或星期五重复此事件

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a>绝对每年

绝对每年模式使事件在每年的同一月份的同一天（例如，4 月 15 日）重复，它基于每次事件之间的年数。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **dayOfMonth** | 必需 | 指定事件发生在每月的哪一天。 |
| **month** | 必需 | 指定事件发生的月份。 |
| **interval** | 必需 | 指定每次事件之间的年数。 |
| **type** | 必需 | 必须设置为 `absoluteYearly`。 |

#### <a name="example"></a>示例

- 在每年的 4 月 15 日重复此事件

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a>相对每年

相对每年模式使事件基于每次事件之间的年数，在特定月份同一相对位置中每周的同一天重复。例如，“每年 11 月的最后一个星期三”。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **daysOfWeek** | 必需 | 指定该事件可以在一周中的哪一天发生。相对年度事件每年仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。 |
| **index** | 可选 | 指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。 可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。 默认值为：`first`。 |
| **month** | 必需 | 指定事件发生的月份。 |
| **interval** | 必需 | 指定每次事件之间的年数。 |
| **type** | 必需 | 必须设置为 `relativeYearly`。 |

#### <a name="examples"></a>示例

- 每年 11 月的最后一个星期三重复此事件

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a>定期范围

重复的第二部分是范围。 它指定模式重复的持续时间。 例如，一个事件可以在发生 10 次后于特定日期结束，也可以不结束。 在 API 中，由 [recurrenceRange 资源](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)表示范围。

**recurrenceRange** 的特定字段是必需还是忽略取决于范围的类型。

> **注意**：即使将字段忽略，仍需验证该字段。 如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。

让我们来看看每个可能的范围类型。

### <a name="numbered-range"></a>编号的范围

编号的范围使事件（基于模式）从开始日期起按固定次数发生。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **numberOfOccurences** | 必需 | 指定事件发生的次数。 必须是正整数。 |
| **recurrenceTimeZone** | 可选 | 指定 **startDate** 属性的时区。 如果未指定，将使用事件时区。 |
| **startDate** | 必需 | 指定开始应用模式的日期。 **startDate** 的值必须与 [事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。 请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。 |
| **type** | 必需 | 必须设置为 `numbered`。 |

#### <a name="examples"></a>示例

- 此事件重复 10 次

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a>结束日期范围

结束日期范围使事件在开始日期和结束日期之间匹配适用模式的所有天数发生。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **endDate** | 必需 | 指定停止应用该模式的日期。请注意，如果日期不符合模式，最后一次会议可能不会在此日期发生。 |
| **recurrenceTimeZone** | 可选 | 指定 **startDate** 和 **endDate** 属性的时区。 如果未指定，将使用事件时区。 |
| **startDate** | 必需 | 指定开始应用模式的日期。 **startDate** 的值必须与 [事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。 请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。 |
| **type** | 必需 | 必须设置为 **endDate**。 |

#### <a name="examples"></a>示例

- 从 2017 年 7 月 1 日到 2017 年 7 月 31 日重复此事件

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a>无结束范围

无结束区域使事件在开始日期后匹配适用模式的所有天数发生。

#### <a name="relevant-properties"></a>相关属性

| 属性 | 相关性 | 说明 |
|----------|-----------|-------------|
| **recurrenceTimeZone** | 可选 | 指定 **startDate** 属性的时区。 如果未指定，将使用事件时区。 |
| **startDate** | 必需 | 指定开始应用模式的日期。 **startDate** 的值必须与 [事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。 请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。 |
| **type** | 必需 | 必须设置为 `noEnd`。 |

#### <a name="examples"></a>示例

- 从 2017 年 5 月 15 日起重复此事件，无结束日期

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a>使用模式和范围创建定期事件

我们已经分别查看了模式和范围，让我们再来了解一下它们如何协同工作以及如何与事件中的 **start** 和 **end** 属性交互。

### <a name="creating-a-recurrence-rule"></a>创建定期规则

如要创建定期规则，必须同时指定模式和范围。 模式类型与范围类型可任意搭配使用。 以下是一些示例。

#### <a name="examples"></a>示例

- **从 2017 年 9 月 4 日开始直到年底，在每周一的下午 1:00 - 1:30 会面**

  - `weekly` 定期模式类型可轻松实现“每周一”的要求。
  - “直到年底”的要求表示 `endDate` 定期范围类型。

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  由于 2017 年 12 月 31 日是周日，因此，此系列的最后一次事件将于 12 月 25 日星期一发生。

- **从 2017 年 8 月 29 日开始，在每两个月的第一个星期四的下午 2:00 - 3:00 会面**

  - 使用相对每月模式可实现“每两个月的第一个星期四”的要求。 “每两个月”部分表示应将 **interval** 设置为 `2`。
  - 由于结束日期没有要求，可使用 `noEnd` 范围类型。

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  由于 **startDate** 的值在 8 月的第一个星期四之后，因此，此系列的第一次事件将在 9 月发生。

## <a name="next-steps"></a>后续步骤
    
- 了解更多关于[与 Outlook 日历集成](outlook-calendar-concept-overview.md)的信息。
- 在日历 API 参考中查看其他定期事件示例：
  - [创建每周发生一次的定期事件](/graph/api/user-post-events?view=graph-rest-1.0#request-3)
  - [创建每日定期事件](/graph/api/user-post-events?view=graph-rest-1.0#request-4)


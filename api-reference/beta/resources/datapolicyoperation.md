---
title: dataPolicyOperation 资源类型
description: 表示提交的数据策略操作。 它包含跟踪操作状态的必要信息。 例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f12d83ace221a64754e4227ff292e780abf7ea82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962628"
---
# <a name="datapolicyoperation-resource-type"></a>dataPolicyOperation 资源类型

命名空间：microsoft.graph

表示提交的数据策略操作。 它包含跟踪操作状态的必要信息。 例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |读取 dataPolicyOperation 对象的属性。|

## <a name="properties"></a>属性

> **注意：** 此资源的所有属性都是只读的。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|表示此数据策略操作的请求使用 ISO 8601 格式以 UTC 时间完成的时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 Null，直到操作完成。|
|id|String| 此操作的唯一键。 |
|状态|dataPolicyOperationStatus| 可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。|
|storageLocation|String|导出请求将数据导出到的 URL 位置。|
|userId|String|操作所针对的用户的 ID。|
|submittedDateTime|DateTimeOffset|表示使用 ISO 8601 格式提交此数据操作请求的时间（UTC 时间）。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|progress|双精度|指定操作的进度。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



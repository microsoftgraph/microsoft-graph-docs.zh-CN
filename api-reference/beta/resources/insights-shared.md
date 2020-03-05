---
title: sharedInsight 资源类型
description: 了解表示与用户共享的文件或由特定用户共享的文件。 支持以下共享文件：
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e6d0304ed73e9452126064ab72e66e6ce3fff0bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495639"
---
# <a name="sharedinsight-resource-type"></a>sharedInsight 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

了解表示与用户共享的文件或由特定用户共享的文件。 支持以下共享文件：

- 直接在电子邮件或会议邀请中附加的文件。
- OneDrive for Business 和 SharePoint 新式附件-存储在 OneDrive for Business 和 SharePoint 中且用户共享为电子邮件中的链接的文件。

**注意**：我们目前正在努力使用数据填充共享 API 的结果。 发布后的第一周可能缺少一些数据。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[共享的列表](../api/insights-list-shared.md) |[sharedInsight](insights-shared.md) 集合| 获取共享文件的列表。|

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明  |
| -------------         |---------------            | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | 共享项目的详细信息。 只读。        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | 可用于在体验中可视化文档的属性。 只读      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | 引用共享文档的属性，例如文档的 url 和类型。 只读       |

## <a name="relationships"></a>关系

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | 实体集合 | 用于导航到已共享的项目。 对于文件附件，类型为*fileAttachment*。 对于链接的附件，类型为*driveItem*。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```

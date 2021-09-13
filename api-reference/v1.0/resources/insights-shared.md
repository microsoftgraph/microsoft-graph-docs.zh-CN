---
title: sharedInsight 资源类型
description: 代表与特定用户共享或由特定用户共享的文件的见解。 支持以下共享文件：
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3e9762c2da54f10e28e0337930972c6a6094ac65
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118584"
---
# <a name="sharedinsight-resource-type"></a>sharedInsight 资源类型

命名空间：microsoft.graph

代表与特定用户共享或由特定用户共享的文件的见解。 支持以下共享文件：

- 直接附加到电子邮件或会议邀请中的文件。
- OneDrive for Business和SharePoint新式附件 - 存储在电子邮件OneDrive for Business SharePoint中作为链接共享的文件。

**注意**：我们目前正在使用数据填充共享 API 的结果。 发布后的第一周可能缺少一些数据。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[共享的列表](../api/insights-list-shared.md) |[sharedInsight](insights-shared.md) 集合| 获取共享文件的列表。|

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明  |
| -------------         |---------------            | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | 有关共享项目的详细信息。 只读。        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | 可用于在体验中可视化文档的属性。 只读      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | 引用共享文档的属性，例如文档的 url 和类型。 只读       |

## <a name="relationships"></a>关系

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | 实体集合 | 用于导航到共享的项目。 对于文件附件，类型为 *fileAttachment*。 对于链接附件，类型为 *driveItem*。 |

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


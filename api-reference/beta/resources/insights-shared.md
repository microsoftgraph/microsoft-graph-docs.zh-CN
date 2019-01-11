---
title: 共享的资源类型
description: 表示文件共享或特定用户洞察。 支持以下共享的文件：
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880610"
---
# <a name="shared-resource-type"></a>共享的资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示文件共享或特定用户洞察。 支持以下共享的文件：

- 邀请电子邮件或会议中的直接附加文件。
- 业务和 SharePoint 的现代附件的文件存储在 OneDrive 中的业务和电子邮件中作为链接共享用户的 SharePoint OneDrive。

**注意**： 我们当前正在填充数据的共享 api 的结果。 可能在发布后第一周中缺少一些数据。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[共享列表](../api/insights-list-shared.md) |[insights_shared](insights-shared.md)集合| 获取共享文件的列表。|

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明  |
| -------------         |---------------            | -------------|
| id                    | 字符串                    | 关系的唯一标识符。 只读。        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | 有关共享项目的详细信息。 只读。        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | 您可以使用可视化中您的体验的文档的属性。 只读      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | 引用的共享文档，如 url 和类型的文档属性。 只读       |

## <a name="relationships"></a>Relationships

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | Entity        | 用于导航到共享的项目。 文件附件的类型为*fileAttachment*。 对于链接附件，类型为*driveItem*。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```

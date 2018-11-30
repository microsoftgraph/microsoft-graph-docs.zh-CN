---
title: 使用资源类型
description: 表示特定用户所使用的文档洞察。 见解返回最相关的文档的用户查看或访问。 这包括文档中的文档：
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047325"
---
# <a name="used-resource-type"></a>使用资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示特定用户所使用的文档洞察。 见解返回最相关的文档的用户查看或访问。 这包括文档中的文档：

- OneDrive for Business
- SharePoint

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[使用列表](../api/insights-list-used.md) |[insights_used](insights-used.md)集合| 获取使用过的文件列表。|

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明  |
| -------------         |---------------            | -------------|
| id                    | 字符串                    | 关系的唯一标识符。 只读。        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | 有关项目时上次查看和修改的用户的信息。 只读。     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | 您可以使用可视化中您的体验的文档的属性。 只读      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | 使用文档，如 url 和的文档类型的引用属性。 只读     |

## <a name="relationships"></a>Relationships

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | 实体        | 用于导航到已使用的项目。 文件附件的类型为*fileAttachment*。 对于链接附件，类型为*driveItem*。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
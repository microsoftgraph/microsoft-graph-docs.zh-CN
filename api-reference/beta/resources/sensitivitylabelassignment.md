---
title: sensitivityLabelAssignment 资源类型
description: 提供有关在SharePoint或OneDrive for Business中分配给文件的敏感度标签的详细信息。
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3f46f0c064bb03286f1d38ba9c915db243acff9f
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917812"
---
# <a name="sensitivitylabelassignment-resource-type"></a>sensitivityLabelAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关在SharePoint或OneDrive for Business中分配给[文件](./driveitem.md)的敏感度标签的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignmentMethod|sensitivityLabelAssignmentMethod|指示标签分配是作为标准还是特权操作自动完成。 可能的值包括 `standard`、`privileged`、`auto`、`unknownFutureValue`。|
|sensitivityLabelId|字符串|分配给文件的敏感度标签的唯一标识符。|
|tenantId|字符串|应用此标签时托管文件的租户的唯一标识符。|

### <a name="sensitivitylabelassignmentmethod-values"></a>sensitivityLabelAssignmentMethod 值

| 成员             | 说明                                    |
|:------------------ |:-----------------------------------------------|
| 标准           | 标签的赋值方法是标准的。|
| 特权         | 标签的赋值方法是特权。 指示标签由用户或管理员手动应用。|
| 自动               | 指示由于配置的策略（例如默认标签或敏感内容的自动分类），系统会自动应用标签。|
| unknownFutureValue | 可变枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|标签|[extractSensitivityLabelsResult](./extractsensitivitylabelsresult.md)|分配给文件的敏感度标签列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitivityLabelAssignment",
  "assignmentMethod": "String",
  "sensitivityLabelId": "String",
  "tenantId": "String"
}
```


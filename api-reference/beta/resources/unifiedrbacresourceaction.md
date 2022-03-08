---
title: unifiedRbacResourceAction 资源类型
description: 表示允许授权主体执行的操作。
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4407c12d18576c6a6ad560588381bc7abd2b4855
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338339"
---
# <a name="unifiedrbacresourceaction-resource-type"></a>unifiedRbacResourceAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示允许授权主体执行的操作。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRbacResourceActions](../api/unifiedrbacresourcenamespace-list-resourceactions.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) 集合|获取 [unifiedRbacResourceAction 对象](../resources/unifiedrbacresourceaction.md) 及其属性的列表。|
|[获取 unifiedRbacResourceAction](../api/unifiedrbacresourceaction-get.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|读取 [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionVerb|字符串|此操作的 HTTP 方法，如 `DELETE`、 `GET`、 `PATCH`、 `POST`、 `PUT`或 `null`。 支持 `$filter` (`eq`) ，但不能用于 `null` 值。 |
|description|String|操作的说明。 支持 `$filter`（`eq`）。 |
|id|String|资源命名空间中操作的唯一标识符，例如 `microsoft.insights-programs-update-patch`。 不能包括斜杠字符 (`/`) 。 不区分大小写。 必需项。 支持 `$filter`（`eq`）。 |
|name|String|资源命名空间中操作的名称，例如 `microsoft.insights/programs/update`。 可以包含斜杠字符 (`/`) 。 不区分大小写。 必需项。 支持 `$filter`（`eq`）。 |
|resourceScopeId|String|未实现。|

## <a name="relationships"></a>关系

无。

<!-- The resourceScope relationship hasn't been implemented but is in the public schema. To unhide this and its related entities and methods once it's implemented.
|Relationship|Type|Description|
|:---|:---|:---|
|resourceScope| [unifiedRbacResourceScope](unifiedrbacresourcescope.md) |Not implemented.|
-->

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceAction",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceAction",
  "id": "String (identifier)",
  "actionVerb": "String",
  "description": "String",
  "name": "String",
  "resourceScopeId": "String"
}
```

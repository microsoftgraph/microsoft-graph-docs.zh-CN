---
title: unifiedRbacResourceNamespace 资源类型
description: 表示角色权限所属的地区的命名空间。
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 85c290fc07c251864507ec34de0a4d6b6027b79e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338406"
---
# <a name="unifiedrbacresourcenamespace-resource-type"></a>unifiedRbacResourceNamespace 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示区域或服务的命名空间，如Azure AD、Intune 和Exchange角色权限的命名空间。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRbacResourceNamespaces](../api/rbacapplicationmultiple-list-resourcenamespaces.md)|[unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) 集合|获取 [unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) 对象及其属性的列表。|
|[获取 unifiedRbacResourceNamespace](../api/unifiedrbacresourcenamespace-get.md)|[unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|读取 [unifiedRbacResourceNamespace 对象的属性和](../resources/unifiedrbacresourcenamespace.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|定义权限的资源命名空间的唯一标识符，例如 `microsoft.aad.b2c`。 必需项。|
|name|String|资源命名空间的名称。 通常，与 **id** 属性同名，例如 `microsoft.aad.b2c`。 必需项。 支持 `$filter`（`eq`、`startsWith`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|resourceActions|[unifiedRbacResourceAction](unifiedrbacresourceaction.md) 集合|允许授权主体执行的操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceNamespace",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceNamespace",
  "id": "String (identifier)",
  "name": "String"
}
```

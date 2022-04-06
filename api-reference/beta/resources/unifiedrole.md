---
title: unifiedRole 资源类型
description: 可通过委派管理员关系分配给 Microsoft 合作伙伴的目录角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8a5c1cc9d450275642e767f7653eea09bcb103f6
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589738"
---
# <a name="unifiedrole-resource-type"></a>unifiedRole 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可通过委派管理员关系分配给 Microsoft 合作伙伴的目录角色。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleDefinitionId|String|目录角色的统一角色定义 ID。 请参阅 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 资源。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRole"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRole",
  "roleDefinitionId": "String"
}
```


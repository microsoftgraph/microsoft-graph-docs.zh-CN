---
title: unifiedRole 资源类型
description: 可以通过委派的管理关系分配给 Microsoft 合作伙伴的目录角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2355770dfdae2209d61903e7160527a57d4e5203
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704415"
---
# <a name="unifiedrole-resource-type"></a>unifiedRole 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以通过委派的管理关系分配给 Microsoft 合作伙伴的目录角色。

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


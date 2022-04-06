---
title: delegatedAdminAccessContainer 资源类型
description: 通过访问分配分配目录角色的管理员访问容器。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0f129195430f51ca3102f38db5730eb36ea4d7a8
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589755"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>delegatedAdminAccessContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过访问分配分配目录角色的管理员访问容器。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessContainerId|String|访问容器的标识符 (例如，安全组) 。 对于"securityGroup"访问容器，这必须是 Microsoft Azure AD租户中安全组的有效 ID。|
|accessContainerType|delegatedAdminAccessContainerType|例如，访问容器 (，安全组) 委派管理员关系分配一个或多个角色。 可能的值是：、`securityGroup``unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessContainer",
  "accessContainerId": "String",
  "accessContainerType": "String"
}
```


---
title: delegatedAdminAccessContainer 资源类型
description: 一个管理员访问容器，通过该容器通过访问分配分配目录角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 330cbb49f1ad78f327b3d00c9b04b16004de2969
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704329"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>delegatedAdminAccessContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个管理员访问容器，通过该容器通过访问分配分配目录角色。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessContainerId|String|访问容器的标识符 (例如，安全组) 。 对于"securityGroup"访问容器，这必须是 Microsoft 合作伙伴租户中Azure AD安全组的有效 ID。|
|accessContainerType|delegatedAdminAccessContainerType|例如，访问容器 (类型，安全组) 通过委派的管理关系分配一个或多个角色。 可能的值为： `securityGroup`. `unknownFutureValue`|

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


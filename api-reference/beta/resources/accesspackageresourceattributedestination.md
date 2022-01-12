---
title: accessPackageResourceAttributeDestination 资源类型
description: 一个抽象类型，用于公开定义将传递用户配置的值的结束系统的对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4d45cff09dd246affd4cc125163c8c435608b14b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865414"
---
# <a name="accesspackageresourceattributedestination-resource-type"></a>accessPackageResourceAttributeDestination 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问包 **的 attributeDestination** 属性的抽象类型。 实际目标将是此复杂类型的子类型。

目前，唯一受支持的子类型是 [accessPackageUserDirectoryAttributeStore](../resources/accesspackageuserdirectoryattributestore.md)。  

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeDestination"
}
```

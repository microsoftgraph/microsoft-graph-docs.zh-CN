---
title: accessPackageResourceAttributeDestination 资源类型
description: 一个抽象类型，用于公开定义将传递用户配置的值的结束系统的对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7254c0910e930cfcb3d96fd1e4f529a6e9551c3
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468333"
---
# <a name="accesspackageresourceattributedestination-resource-type"></a>accessPackageResourceAttributeDestination 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 [accessPackageResourceAttribute](accesspackageresourceattribute.md) **的 attributeDestination** 属性的抽象类型。 实际目标将是此复杂类型的子类型。

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

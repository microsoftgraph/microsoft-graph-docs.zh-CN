---
title: accessPackageResourceAttributeQuestion 资源类型
description: 用于定义提供给最终用户的问题的资源，以获取要传递给最终系统或请求审批者的属性值。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a5731575e5368e50699b57da419b357d145f786f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865413"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>accessPackageResourceAttributeQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于定义提供给最终用户的问题的资源，以获取要传递给最终系统或请求审批者的属性值。

继承自 [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|question|accessPackageQuestion|为了获取属性的值而询问的问题|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
  "question": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

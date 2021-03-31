---
title: servicePrincipalIdentity 资源类型
description: 为服务主体标识创建模型。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a49adab87ac5ebe7b8eddf106d8d38c4e15acd11
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469738"
---
# <a name="serviceprincipalidentity-resource-type"></a>servicePrincipalIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为服务主体标识创建模型。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appId|String| 服务主体的应用程序标识符。 |
|displayName|String| 服务显示名称标识的组。 继承自 [标识](../resources/identity.md)。 |
|id|String| 服务主体标识的标识符。 继承自 [标识](../resources/identity.md)。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```

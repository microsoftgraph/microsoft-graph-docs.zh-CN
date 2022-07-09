---
title: servicePrincipalIdentity 资源类型
description: 为服务主体标识创建模型。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f2daece3e3f9fb01c58a2470aa667da7e62ce4ef
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697926"
---
# <a name="serviceprincipalidentity-resource-type"></a>servicePrincipalIdentity 资源类型

命名空间：microsoft.graph

为服务主体标识创建模型。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appId|String|服务主体的应用程序标识符。|
|displayName|String|服务主体标识的显示名称。 继承自 [标识](../resources/identity.md)|
|id|String|服务主体标识的标识符。 继承自 [标识](../resources/identity.md)|

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

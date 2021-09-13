---
title: servicePrincipalIdentity 资源类型
description: 为服务主体标识创建模型。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae9d82ce65b7a6e8c82e0377df89939b9219f3db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108826"
---
# <a name="serviceprincipalidentity-resource-type"></a>servicePrincipalIdentity 资源类型

命名空间：microsoft.graph

为服务主体标识创建模型。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appId|String|服务主体的应用程序标识符。|
|displayName|String|服务显示名称标识的标识。 继承自 [标识](../resources/identity.md)|
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

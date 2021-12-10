---
title: authenticationMethodsRoot 资源类型
description: 用于身份验证方法资源的Azure AD属性的容器。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e01fe33d73d67058bf765d3562c77ea657630ea6
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403198"
---
# <a name="authenticationmethodsroot-resource-type"></a>authenticationMethodsRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于身份验证方法资源的Azure AD属性的容器。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 唯一标识符。 继承自 [实体](../resources/entity.md)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRoot",
  "id": "String (identifier)"
}
```
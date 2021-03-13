---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 691184b1dfbf0323204debd70488d232d77b4f7a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761133"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>authenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示身份验证方法策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略名称。|
|state|authenticationMethodState|策略的状态。 可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

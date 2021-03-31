---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26d0cd948a69968a7d45b3406b3da7109ffc3f18
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469127"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>authenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

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

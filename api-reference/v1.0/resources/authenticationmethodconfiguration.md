---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 27f0c8e809b88ad77a12a0f5e28acb9eeed953c9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126987"
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

---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 658e27e4fe75424f4bd39cc6c3a76255e70c4d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988805"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>selfServiceSignUpAuthenticationFlowConfiguration 资源类型


命名空间：microsoft.graph

表示与自助注册相关的配置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:-------|:---|:----------|
|isEnabled|Boolean|指示是启用还是禁用自助注册流。 默认值为 `false`。 此属性不是一个注册表项。 必填。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```



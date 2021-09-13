---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 735803c579f79e9f27f81c53fd9e3fd5ce94e84a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067015"
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

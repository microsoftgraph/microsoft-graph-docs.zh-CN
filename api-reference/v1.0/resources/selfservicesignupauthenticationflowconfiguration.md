---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 96800f7b3ef2509cf52a302409b03cfc2d3fd62dee864da99ecf6ecf8e3bde7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126282"
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

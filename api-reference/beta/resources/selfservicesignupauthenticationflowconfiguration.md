---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3bab808249ee7417d721e68dbd2a172c71daf593
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696881"
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



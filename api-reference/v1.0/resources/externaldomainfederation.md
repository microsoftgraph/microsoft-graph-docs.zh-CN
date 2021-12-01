---
title: externalDomainFederation 资源类型
description: externalDomainFederation 类型将已配置的标识提供程序标识为已连接组织的标识源的非租户域。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: af47b7516e656ad85cbe1f8ef2fde3f0681ee89c
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242328"
---
# <a name="externaldomainfederation-resource-type"></a>externalDomainFederation 资源类型

命名空间：microsoft.graph


在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 该值指示此类型将已配置的标识提供程序标识为已连接组织的 `@odata.type` `#microsoft.graph.externalDomainFederation` 标识源的域。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|标识源的名称，通常也是域名。 只读。 |
|domainName|String|域名。 只读。 |
|issuerUri|String|传入联盟的 issuerURI。 只读。 |

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalDomainFederation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainFederation",
  "issuerUri": "String",
  "domainName": "String",
  "displayName": "String"
}
```



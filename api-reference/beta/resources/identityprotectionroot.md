---
title: identityProtectionRoot 资源类型
description: Microsoft 导航属性容器Graph标识保护资源。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 90b8de67f24c650f1a4f6832979f5d669f9af57e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519446"
---
# <a name="identityprotectionroot-resource-type"></a>identityProtectionRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 导航属性的容器Graph[标识保护](identityprotection-overview.md)资源。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|riskDetections|[riskDetection](../resources/riskdetection.md) 集合| Identity Protection Azure AD中的风险检测，以及检测的相关信息。|
|riskyUsers|[riskyUser](../resources/riskyuser.md) 集合|Identity Protection 标记为处于风险Azure AD用户。 |
|riskyServicePrincipals| [riskyServicePrincipal](riskyserviceprincipal.md) 集合 | Azure AD存在风险的服务主体。 |
|servicePrincipalRiskDetections| [servicePrincipalRiskDetection](serviceprincipalriskdetection.md) 集合 | 表示有关在租户中检测到的风险服务Azure AD的信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProtectionRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProtectionRoot"
}
```


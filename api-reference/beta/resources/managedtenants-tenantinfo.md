---
title: tenantInfo 资源类型
description: 表示托管租户的信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 96b899eeb6e16ef42b94f0632501e562db0a460f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791852"
---
# <a name="tenantinfo-resource-type"></a>tenantInfo 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantInfo",
  "tenantId": "String"
}
```

---
title: managementTemplateDetailedInfo 资源类型
description: 表示管理模板的详细信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7ece5863f33f447a6e79ea75e1959ea7011b0c32
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861349"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a>managementTemplateDetailedInfo 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示管理模板的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|managementCategory|管理模板的管理类别。 可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。 必需。 只读。|
|displayName|String|管理显示名称模板的模板。 必需。 只读。|
|managementTemplateId|String|管理模板的唯一标识符。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```

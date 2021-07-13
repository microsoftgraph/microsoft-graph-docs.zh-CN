---
title: managementTemplateDetailedInfo 资源类型
description: 表示管理模板的详细信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402360"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a>managementTemplateDetailedInfo 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示管理模板的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|managementCategory|管理模板的管理类别。 可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。 必填。 只读。|
|displayName|String|管理显示名称的表单。 必填。 只读。|
|managementTemplateId|String|管理模板的唯一标识符。 必填。 只读。|

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

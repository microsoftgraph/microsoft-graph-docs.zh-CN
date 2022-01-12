---
title: managementActionInfo 资源类型
description: 表示管理操作的引用信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: afd219145ae5a58048985290bc1a01e9e7cccf09
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860955"
---
# <a name="managementactioninfo-resource-type"></a>managementActionInfo 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示管理操作的引用信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managementActionId|String|管理操作标识符。 必需。 只读。|
|managementTemplateId|String|管理模板的标识符。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionInfo",
  "managementTemplateId": "String",
  "managementActionId": "String"
}
```

---
title: azureAdJoinPolicy 资源类型
description: 表示使用 Azure AD Join 控制设备注册的 Azure Active Directory 租户的策略范围。
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 46abc16a3982f7f9d22881f02cf13225d1daadcf
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66689977"
---
# <a name="azureadjoinpolicy-resource-type"></a>azureAdJoinPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure ACTIVE Directory (Azure AD) 租户的策略范围，该租户控制用户和组使用 Azure AD Join 向组织注册设备标识的能力。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|allowedGroups|字符串集合|策略范围内的组的标识符。 Required when the **appliesTo** property is set to `selected`. |
|allowedUsers|String collection|策略范围内的用户的标识符。 Required when the **appliesTo** property is set to `selected`.|
|appliesTo|policyScope|指定是阻止还是允许对策略范围进行精细控制。 可能的值是： `0` (含义 `none`) 、 `1` (含义 `all`) 、 `2` (含义 `selected`)  (`3` 含义 `unknownFutureValue`) 。 <br/><br/>默认值为 `1`。 设置为 `2`时，必须至少在 **allowedUsers** 或 **allowedGroups** 中指定一个用户或组标识符。  将此属性设置为 `0` 或 `1` 删除 **allowedUsers** 和 **allowedGroups** 中的所有标识符。|
|isAdminConfigurable|Boolean|指定管理员是否可配置此策略范围。默认值为 `false`. 当管理员启用了Intune (MEM) 来管理设备时，此属性设置为`false`并 **应用到** 默认值，以`1` (表示`all`) 。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdJoinPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureAdJoinPolicy",
  "appliesTo": "String",
  "isAdminConfigurable": "Boolean",
  "allowedUsers": [
    "String"
  ],
  "allowedGroups": [
    "String"
  ]
}
```

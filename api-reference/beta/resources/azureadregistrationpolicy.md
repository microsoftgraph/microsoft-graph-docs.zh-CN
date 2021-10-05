---
title: azureADRegistrationPolicy 资源类型
description: 表示使用已注册的 Azure AD Azure Active Directory控制设备注册的租户的策略范围。
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: dd6c0b138a46dc5759811a6e5865327a75016ddc
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127914"
---
# <a name="azureadregistrationpolicy-resource-type"></a>azureADRegistrationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD Azure Active Directory (租户的策略) ，该租户控制用户和组使用已注册 **的 Azure AD** 向组织注册设备标识的能力。 有关详细信息，请参阅[什么是设备标识？。](/azure/active-directory/devices/overview)

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|allowedGroups|字符串集合| 策略范围内组的标识符。 当 **appliesTo** 属性设置为 时，此属性或 **allowedUsers** 是必需的 `selected` 。 |
|allowedUsers|String collection| 策略范围内用户的标识符。 当 **appliesTo** 属性设置为 时，此属性或 **allowedGroups** 是必需的 `selected` 。 |
|appliesTo|policyScope|指定是阻止还是允许对策略范围的精细控制。 可能的值包括 `0` `none` ： (、) 、 () 、 () 、 () 。 `1` `all` `2` `selected` `3` `unknownFutureValue` <br/><br/>默认值为 `1`。 设置为 `2` 时，必须在 **allowedUsers** 或 **allowedGroups** 中指定至少一个用户或组标识符。  将此属性设置为 `0` 或 `1` 同时删除 **allowedUsers** 和 **allowedGroups 中的所有标识符**。|
|isAdminConfigurable|布尔|指定管理员是否可配置此策略作用域。默认值为 `false` 。 当管理员启用 Intune (MEM) 管理设备时，此属性将设置为 并 `false` **应用默认值** 为 (`1` 表示 `all`) 。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureADRegistrationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADRegistrationPolicy",
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

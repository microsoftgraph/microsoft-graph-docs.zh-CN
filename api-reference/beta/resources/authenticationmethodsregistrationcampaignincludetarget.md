---
title: authenticationMethodsRegistrationCampaignIncludeTarget 资源类型
description: 允许提示用户和用户组设置目标身份验证方法。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682878"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>authenticationMethodsRegistrationCampaignIncludeTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示面向身份验证方法注册活动的用户和组。 只有策略启用以设置身份验证方法的用户和组作为目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象标识符。|
|targetedAuthenticationMethod|String|提示用户注册的身份验证方法。 值必须为 `microsoftAuthenticator` 。|
|targetType|authenticationMethodTargetType|身份验证方法目标的类型。 可取值为：`user`、`group`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```

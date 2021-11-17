---
title: authenticationMethodsRegistrationCampaignIncludeTarget 资源类型
description: 允许提示用户和用户组设置目标身份验证方法。
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 51f6e1a9842c05a8fb88a92b38cb0c54fbe0d91e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994711"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>authenticationMethodsRegistrationCampaignIncludeTarget 资源类型

命名空间：microsoft.graph

表示面向身份验证方法注册活动的用户和组。 只有策略启用以设置身份验证方法的用户和组作为目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户或组Azure Active Directory标识符。|
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

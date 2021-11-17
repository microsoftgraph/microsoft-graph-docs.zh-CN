---
title: authenticationMethodsRegistrationCampaign 资源类型
description: 表示用于运行市场活动以推送用户设置目标身份验证方法的设置。
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71de25c16e357ade6aca9f2bb7fd5100cf8af7cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019158"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a>authenticationMethodsRegistrationCampaign 资源类型

命名空间：microsoft.graph

表示用于运行市场活动以推送用户设置目标身份验证方法的设置。 用户成功完成 MFA 质询后，系统会提示他们设置身份验证方法。 仅适用于 MFA Microsoft Authenticator应用。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|excludeTargets|[excludeTarget](../resources/excludetarget.md) 集合|系统提示他们设置身份验证方法时排除的用户和用户组。|
|includeTargets|[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) 集合|提示设置身份验证方法的用户和用户组。|
|snoozeDurationInDays|Int32|指定用户在选择"Not now"并暂停提示时再次看到提示的天数。 最小值：0 天。 最大值：14 天。 如果值为"0"，则每次尝试 MFA 时都会提示用户。|
|state|advancedConfigState|启用或禁用该功能。 可能的值是：`default`、`enabled`、`disabled`、`unknownFutureValue`。 当配置尚未明确设置并使用设置的默认行为时，Azure Active Directory `default` 值。 默认值为 `disabled`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Int32",
  "state": "String"
}
```

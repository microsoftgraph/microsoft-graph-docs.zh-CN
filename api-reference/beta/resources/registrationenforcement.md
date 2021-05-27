---
title: registrationEnforcement 资源类型
description: 在登录时强制注册。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86d3e974ccfebdf0011c9c19f881096e3fb2ba40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682870"
---
# <a name="registrationenforcement-resource-type"></a>registrationEnforcement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在登录时强制注册。 目前，这仅用于提醒用户使用"authenticationMethodsRegistrationCampaign" (Microsoft Authenticator) 设置目标身份验证方法。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationMethodsRegistrationCampaign|[authenticationMethodsRegistrationCampaign](../resources/authenticationmethodsregistrationcampaign.md)|开展市场活动以提醒用户设置目标身份验证方法。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```

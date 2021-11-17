---
title: registrationEnforcement 资源类型
description: 在登录时强制注册。
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e46661280fac283123dde6c3820f68911658a6a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019149"
---
# <a name="registrationenforcement-resource-type"></a>registrationEnforcement 资源类型

命名空间：microsoft.graph

在登录时强制注册。 这当前只能用于提醒用户设置目标身份验证方法 (例如，Microsoft Authenticator) 使用 `authenticationMethodsRegistrationCampaign` 。

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

---
title: authenticationMethodsRoot 资源类型
description: 用于 Azure AD 身份验证方法资源的导航属性的容器。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: cc86e2ff67f7c628406aa90aca5bd00d03101272
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820481"
---
# <a name="authenticationmethodsroot-resource-type"></a>authenticationMethodsRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 Azure AD 身份验证方法资源的导航属性的容器。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 唯一标识符。 继承自 [entity](../resources/entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| 表示用户的身份验证方法的状态，包括哪些方法已注册，哪些功能是用户注册的，哪些功能能够 (，例如多重身份验证、自助式密码重置和无密码身份验证) 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRoot",
  "id": "String (identifier)"
}
```
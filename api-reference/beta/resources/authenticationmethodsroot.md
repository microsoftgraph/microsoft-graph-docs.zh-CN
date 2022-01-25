---
title: authenticationMethodsRoot 资源类型
description: 用于身份验证方法资源的Azure AD属性的容器。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: def78eddd43cdb7ea738d32e25c8d90adb23fbc4
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201685"
---
# <a name="authenticationmethodsroot-resource-type"></a>authenticationMethodsRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于身份验证方法资源的Azure AD属性的容器。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串| 唯一标识符。 继承自 [实体](../resources/entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| 表示用户的身份验证方法的状态，包括注册哪些方法以及用户注册哪些功能 (如多重身份验证、自助服务密码重置和无密码身份验证) 。|

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
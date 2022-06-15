---
title: temporaryAccessPassAuthenticationMethod 资源类型
description: 表示注册给用户的临时访问通行证。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 136df8006925470d139c7c94f3d7a2c3e0ff35be
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094066"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>temporaryAccessPassAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册给用户的临时访问通行证。 临时访问密码是一个时间限制的密码，用作强凭据并允许载入无密码凭据。 可为 **temporaryAccessPassAuthenticationMethod** 配置的可用性和设置取决于 [临时访问传递方法策略](temporaryaccesspassauthenticationmethodconfiguration.md)。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/authentication-list-temporaryaccesspassmethods.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 集合|检索用户的 **临时AccessPassAuthenticationMethod** 对象及其属性的列表。 用户只能有一个临时访问传递身份验证方法。|
|[创建](../api/authentication-post-temporaryaccesspassmethods.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|创建用户的 **temporaryAccessPassAuthenticationMethod** 对象。|
|[获取](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|检索用户的 **temporaryAccessPassAuthenticationMethod** 对象的属性。|
|[删除](../api/temporaryaccesspassauthenticationmethod-delete.md)|无|删除用户的 **temporaryAccessPassAuthenticationMethod** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建临时访问通行证的日期和时间。|
|id|String|注册给此用户的临时访问通行证的标识符。 继承自 [entity](../resources/entity.md)。|
|isUsableOnce|Boolean|确定传递是否仅限于一次性使用。 如果 `true`可以使用传递一次，则 `false`可在临时访问传递生存期内多次使用该传递。|
|isUsable|布尔值|身份验证方法的状态，指示用户当前是否可用。|
|lifetimeInMinutes|Int32|从 **startDateTime 开始**，临时访问传递的生存期（以分钟为单位）。 必须介于 10 到 43200 之间，包括 (等效于 30 天) 。|
|methodUsabilityReason|String|有关可用性状态 (的详细信息 **) 。** 原因可能包括： `EnabledByPolicy`， `DisabledByPolicy`， `Expired`， `NotYetValid`， 。 `OneTimeUsed`|
|startDateTime|DateTimeOffset|临时访问通行证可供使用的日期和时间以及`true`何时强制使用。|
|temporaryAccessPass|String|用于身份验证的临时访问通行证。 仅在创建新的 **temporaryAccessPassAuthenticationMethod** 对象时返回;隐藏在后续读取操作中，并随 GET 一样 `null` 返回。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```

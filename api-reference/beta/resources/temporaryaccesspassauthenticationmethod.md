---
title: temporaryAccessPassAuthenticationMethod 资源类型
description: 表示注册到用户的临时访问传递。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bd5bd1ab118d7ec5c7443c47bda1ea614f31bf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442805"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>temporaryAccessPassAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册到用户的临时访问传递。 临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/temporaryaccesspassauthenticationmethod-list.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 集合|检索用户的临时 **AccessPassAuthenticationMethod** 对象及其属性的列表。 用户只能有一个临时访问传递身份验证方法。|
|[创建](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|创建用户 **的临时AccessPassAuthenticationMethod** 对象。|
|[获取](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|检索用户的临时 **AccessPassAuthenticationMethod 对象** 的属性。||
|[删除](../api/temporaryaccesspassauthenticationmethod-delete.md)|无|删除用户 **的临时AccessPassAuthenticationMethod** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|注册到此用户的临时访问传递的标识符。|
|temporaryAccessPass|String|用于进行身份验证的临时AccessPass。 仅在新建 temporaryAccessPass 时返回;作为 NULL 与 GET 一起返回。|
|createdDateTime|DateTimeOffset|创建 temporaryAccessPass 的日期和时间。|
|startDateTime|DateTimeOffset|temporaryAccessPass 可供使用的日期和时间。|
|lifetimeInMinutes|Int32|temporaryAccessPass 的生存期（以分钟计，从 startDateTime 开始）。 最少 10 天，最多 43200 (相当于 30 天) 。|
|isUsableOnce|布尔|确定传递是否限制为一次使用。 如果 `true` ，则一次可以使用传递;如果 `false` ，可以在 temporaryAccessPass 生存期内多次使用传递。|
|isUsable|布尔|指示用户当前是否可用身份验证方法的状态。|
|methodUsabilityReason|String|有关可用性状态的详细信息 (可用性) 。 原因可能包括： `enabledByPolicy` ， `disabledByPolicy` ， ， `expired` `notYetValid` `oneTimeUsed` 。|


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

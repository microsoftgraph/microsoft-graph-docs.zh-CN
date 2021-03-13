---
title: temporaryAccessPassAuthenticationMethod 资源类型
description: 表示注册到用户的临时访问通道。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c118978f9e7c8a7c3aa127ba12aba48f2cfe362
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760958"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>temporaryAccessPassAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册到用户的临时访问通道。 临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/temporaryaccesspassauthenticationmethod-list.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 集合|检索用户的临时 **AccessPassAuthenticationMethod** 对象及其属性的列表。 用户只能有一个临时访问传递身份验证方法。|
|[创建](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|创建用户 **的临时AccessPassAuthenticationMethod** 对象。|
|[Get](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|检索用户 **temporaryAccessPassAuthenticationMethod 对象** 的属性。||
|[删除](../api/temporaryaccesspassauthenticationmethod-delete.md)|无|删除用户 **的临时AccessPassAuthenticationMethod** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|注册到此用户的临时访问传递的标识符。|
|temporaryAccessPass|String|用于进行身份验证的 temporaryAccessPass。 仅在新建 temporaryAccessPass 时返回;与 GET 一起返回为 NULL。|
|createdDateTime|DateTimeOffset|创建 temporaryAccessPass 的日期和时间。|
|startDateTime|DateTimeOffset|temporaryAccessPass 可供使用的日期和时间。|
|lifetimeInMinutes|Int32|temporaryAccessPass 的生存期，以分钟计，从 startDateTime 开始。 最少 10 天，最多 43200 (相当于 30 天) 。|
|isUsableOnce|布尔|确定是否将传递限制为一次使用。 如果 `true` 为 ，则传递可以使用一次;如果 为 ，则 pass 可以在 `false` temporaryAccessPass 生存期内多次使用。|
|isUsable|布尔|身份验证方法的状态，指示它当前是否由用户使用。|
|methodUsabilityReason|String|有关可用性状态的详细信息 (isUsable) 。 原因可能包括 `enabledByPolicy` `disabledByPolicy` `expired` ：、、、、。 `notYetValid` `oneTimeUsed`|


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

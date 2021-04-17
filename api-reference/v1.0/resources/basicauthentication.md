---
title: basicAuthentication 资源类型
description: 表示在 API 调用中使用基本身份验证的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9bb61e297a6a668631da654383e13ee1dbf8ef79
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882395"
---
# <a name="basicauthentication-resource-type"></a>basicAuthentication 资源类型

命名空间：microsoft.graph

表示在 API 调用中使用 HTTP 基本身份验证的配置，这需要用户名和密码。 用户名和密码作为授权标头发送，其中 用户名：password 是 `Basic {value}` `value` base 64 编码版本。

继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|username|String| 用户名。 |
|密码|String| 密码。 响应中不会返回它。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```

---
title: basicAuthentication 资源类型
description: 表示在 API 调用中使用基本身份验证的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720154"
---
# <a name="basicauthentication-resource-type"></a>basicAuthentication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 API 调用中使用 HTTP 基本身份验证的配置，这需要用户名和密码。 用户名和密码作为授权标头发送，就像用户名：password 的 `Basic {value}` `value` base 64 编码版本一样。

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

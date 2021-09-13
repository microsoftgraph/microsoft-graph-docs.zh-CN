---
title: basicAuthentication 资源类型
description: 表示在 API 调用中使用基本身份验证的配置。
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9749d179ffa33020b73747e46ed21add6eb9316d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019396"
---
# <a name="basicauthentication-resource-type"></a>basicAuthentication 资源类型

命名空间：microsoft.graph

表示在 API 调用中使用 HTTP 基本身份验证的配置，这需要用户名和密码。 用户名和密码作为授权标头发送，因为 `Basic {value}` 其中是 `value` 用户名：password 的 base 64 编码版本。

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

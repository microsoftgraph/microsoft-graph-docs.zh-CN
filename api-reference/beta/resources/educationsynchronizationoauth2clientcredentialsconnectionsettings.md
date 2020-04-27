---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序，则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d38853e40d8f88bf4aa8323395848185793cc42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500091"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

如果要使用[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)连接到数据提供程序，则此连接设置类型应用于设置配置文件。

派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **tokenUrl** | String | 用于获取数据提供程序的访问令牌的 URL。 |
| **scope** | String | [访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```

---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序，则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00e1e531ff33f28a2e63f76925cd0b4e7759696b
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434905"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

如果要使用[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)连接到数据提供程序，则此连接设置类型应用于设置配置文件。

派生自[educationSynchronizationConnectionSettings]。

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | 字符串 | 用于连接到提供程序的客户端 ID。 继承自[educationSynchronizationConnectionSettings]。                    |
| clientSecret | 字符串 | 用于对与提供程序的连接进行身份验证的客户端密码。 继承自[educationSynchronizationConnectionSettings]。 |
| tokenUrl     | 字符串 | 用于获取数据提供程序的访问令牌的 URL。                                                                        |
| scope        | String | 访问请求的范围（请参阅[RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)）。                          |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

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

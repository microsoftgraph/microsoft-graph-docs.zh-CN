---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序，则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dfe0a2fda8d49bd003a6ea2c23eb6a31ce619234
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289437"
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

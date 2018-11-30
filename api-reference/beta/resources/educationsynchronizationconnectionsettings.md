---
title: educationSynchronizationConnectionSettings 资源类型
description: '代表提供商连接设置。 这样，系统知道如何连接到提供程序的 Api。 '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045736"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表提供商连接设置。 这样，系统知道如何连接到提供程序的 Api。 

> **注意：** 此复杂类型是抽象类。 引用的特定类型的列出的连接设置。

## <a name="derived-types"></a>派生的类型
| 类型 | 说明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | 使用此类型提供 OAuth1 连接设置。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | 使用此类型提供 OAuth2 客户端凭据授予连接设置。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **clientId** | 字符串 |  用于连接到提供程序的客户端 ID。 |
| **clientSecret** | 字符串 |  验证连接到提供程序的客户端机密。 |
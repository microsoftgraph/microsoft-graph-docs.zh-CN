---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334104"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 api。 

> **注意:** 此复杂类型是抽象的。 请参阅列出的特定类型的连接设置。

## <a name="derived-types"></a>派生类型
| 类型 | 说明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | 使用此类型可提供 OAuth1 连接设置。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | 使用此类型可提供 OAuth2 客户端凭据授予连接设置。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **clientId** | String |  用于连接到提供程序的客户端 ID。 |
| **clientSecret** | String |  用于对与提供程序的连接进行身份验证的客户端密码。 |

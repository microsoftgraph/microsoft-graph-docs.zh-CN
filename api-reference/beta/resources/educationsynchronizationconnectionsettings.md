---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 449dc1c4265355d55e6d3ceb51fe86be9f84ac31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979558"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 Api。

> [!NOTE]
> 此复杂类型是抽象的。 请参阅列出的特定类型的连接设置。

## <a name="derived-types"></a>派生类型

| 类型                                                                                                                                      | 说明                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | 使用此类型可提供 OAuth1 连接设置。                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | 使用此类型可提供 OAuth2 客户端凭据授予连接设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | 字符串 | 用于连接到提供程序的客户端 ID。                    |
| clientSecret | 字符串 | 用于对与提供程序的连接进行身份验证的客户端密码。 |



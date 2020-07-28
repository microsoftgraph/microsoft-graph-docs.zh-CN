---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 71da1acbd9910757375acbc22dda63f412f459b2
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434877"
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

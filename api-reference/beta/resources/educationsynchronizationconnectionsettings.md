---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这允许系统了解如何连接到提供程序 API。 '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4885c2b661d2346eb80d274243c9b15d58769407
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695277"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示提供程序连接设置。 这允许系统了解如何连接到提供程序 API。

> [!NOTE]
> 此复杂类型为抽象类型。 请参阅列出的特定类型的连接设置。

## <a name="derived-types"></a>派生类型

| 类型                                                                                                                                      | 说明                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | 使用此类型可提供 OAuth1 连接设置。                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | 使用此类型可提供 OAuth2 客户端凭据授予连接设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | 字符串 | 用于连接到提供程序的客户端 ID。                    |
| clientSecret | 字符串 | 用于验证与提供程序的连接的客户端密码。 |

## <a name="json-representation"></a>JSON 表示形式

下面是此资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
   truncated: true,
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings"
}-->

```json
{}
```

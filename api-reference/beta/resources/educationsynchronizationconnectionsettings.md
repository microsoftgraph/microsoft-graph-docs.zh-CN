---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这允许系统了解如何连接到提供程序 API。 '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7b64b52946e2391378a34ee3cba3db852d61666d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445898"
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
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings"
}-->

```json
{}
```

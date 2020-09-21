---
title: educationSynchronizationOAuth1ConnectionSettings 资源
description: 当 OAuth1 用于连接到数据提供程序时，此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a73876185469ab762a08f409028880a4f7234d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989626"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>educationSynchronizationOAuth1ConnectionSettings 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当 OAuth1 用于连接到数据提供程序时，此连接设置类型应用于设置配置文件。

派生自 [educationSynchronizationConnectionSettings]。

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | 字符串 | 用于连接到提供程序的客户端 ID。 继承自 [educationSynchronizationConnectionSettings]。                    |
| clientSecret | 字符串 | 用于对与提供程序的连接进行身份验证的客户端密码。 继承自 [educationSynchronizationConnectionSettings]。 |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```



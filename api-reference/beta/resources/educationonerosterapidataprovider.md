---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca3341c84b79ff25e55be1abf5a8a5a031e84b02
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290383"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在将[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **connectionUrl** | String | 指向 OneRoster 实例的连接 URL。 |
| **schoolsIds** | String collection |  要同步的学校 sourcedIds 的列表。 |
| **providerName** | String | 由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义的 OneRoster 服务提供程序名称。 |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | OneRoster 实例的连接设置。 应为[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)的类型类型。 |
| **操作** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 要应用于同步配置文件的可选自定义项。|

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->
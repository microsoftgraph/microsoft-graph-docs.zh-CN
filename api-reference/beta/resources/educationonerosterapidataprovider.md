---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ea02186b7d9bd7bed14c6ea5b46023da81814f07
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791060"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在将[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性           | 类型                                         | 说明                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | String                                       | 指向 OneRoster 实例的连接 URL。                                                         |
| providerName       | String                                       | 由[OneRoster 规范][oneroster]定义的 OneRoster 服务提供程序名称。           |
| schoolsIds         | String collection                            | 要同步的[学校/组织][orgs]的列表 `sourcedId` 。                                                   |
| termIds            | String collection                            | 要同步的[学术会话][terms]的列表。                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | OneRoster 实例的[oauth 1.0][onerosteroauth1]或[oauth 2.0][onerosteroauth2]设置。 |
| 操作     | [educationSynchronizationCustomizations]）    | 要应用于同步配置文件的可选自定义项。                                  |

> [!IMPORTANT]
> OneRoster 使用学术会议，而不是一年的时间来细分其数据。 此细分在学校数据同步 UI 中被抽象掉，而不是在此 API 中。 您需要调用 OneRoster `/terms` 终结点以获取学术会话 id 的集合，以便填充该 `termIds` 集合。

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

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
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
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

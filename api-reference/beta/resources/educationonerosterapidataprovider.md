---
title: educationOneRosterApiDataProvider 资源
description: 用于将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2c90c7132f6e51b84e987cf6bda63baacc60b8ba
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080419"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于将 [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) 用作输入源时设置学校数据同步配置文件。

派生自 [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性           | 类型                                         | 说明                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | String                                       | OneRoster 实例的连接 URL。                                                         |
| providerName       | String                                       | OneRoster 服务提供程序名称，由 [OneRoster 规范定义][oneroster]。           |
| schoolsIds         | String collection                            | 要同步 [的学校/组织][orgs] `sourcedId` 列表。                                                   |
| termIds            | String collection                            | 要同步 [的学院课程][terms] 列表。                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | OneRoster 实例的 [OAuth 1.0][onerosteroauth1] 或 [OAuth 2.0][onerosteroauth2] 设置。 |
| 自定义项     | [educationSynchronizationCustomizations]    | 要应用于同步配置文件的可选自定义。                                  |

> [!IMPORTANT]
> OneRoster 使用学术课程（而不是一个学校年份）来划分数据。 此分段在 UI 中抽象学校数据同步，而不是此 API。 你将需要调用 OneRoster 终结点，获取学院会话 `/terms` 的 ID 集合，以便填充 `termIds` 该集合。

[educationSynchronizationConnectionSettings]: educationsynchronizationconnectionsettings.md
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
  "@odata.type&quot;: &quot;microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  },
  "customizations": {
    "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
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
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.ediscovery.settings"
  ]
}-->



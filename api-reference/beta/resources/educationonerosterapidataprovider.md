---
title: educationOneRosterApiDataProvider 资源
description: 用于将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1445a6c1584ffff803a67939e02b3366bfbd50f3
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291097"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于将 [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) 用作输入源时设置学校数据同步配置文件。

派生自 [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性           | 类型                                         | 说明                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | 字符串                                       | OneRoster 实例的连接 URL。                                                         |
| providerName       | String                                       | OneRoster 服务提供程序名称，由 [OneRoster 规范定义][oneroster]。           |
| schoolsIds         | 字符串集合                            | 要同步[的学校/组织][orgs]`sourcedId`列表。                                                   |
| termIds            | 字符串集合                            | 要同步 [的学院课程][terms] 列表。                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | OneRoster 实例的 [OAuth 1.0][onerosteroauth1] 或 [OAuth 2.0][onerosteroauth2] 设置。 |
| 自定义项     | [educationSynchronizationCustomizations]    | 要应用于同步配置文件的可选自定义。                                  |

> [!IMPORTANT]
> OneRoster 使用学术课程而不是一个学校年份来划分数据。 此分段在 UI 中抽象学校数据同步，而不是此 API。 你将需要调用 OneRoster `/terms` 终结点，获取学院会话的 ID 集合，以便填充该 `termIds` 集合。

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
  truncated: true,
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
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  truncated: true,
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



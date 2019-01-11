---
title: educationOneRosterApiDataProvider 资源
description: 用于 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: a99343ed8026eda9ecf56925986f4a0bfe10b3ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858154"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider 资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

用于[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **connectionUrl** | 字符串 | 连接到 OneRoster 实例 URL。 |
| **schoolsIds** | String 集合 |  学校 sourcedIds 同步的列表。 |
| **providerName** | 字符串 | 由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义 OneRoster 服务提供商的名称。 |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | OneRoster 实例的连接设置。 应类型[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)。 |
| **自定义项** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 可选自定义要应用于同步配置文件。|

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```

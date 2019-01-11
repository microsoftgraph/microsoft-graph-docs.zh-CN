---
title: educationSynchronizationOAuth1ConnectionSettings 资源
description: 当 OAuth1 要用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。
localization_priority: Normal
ms.openlocfilehash: 30c4abce27b1b9593346bcb0392581eb83c7830e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894150"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>educationSynchronizationOAuth1ConnectionSettings 资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

当 OAuth1 要用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。

派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。

## <a name="properties"></a>属性

此类型不公开任何其他属性。

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```

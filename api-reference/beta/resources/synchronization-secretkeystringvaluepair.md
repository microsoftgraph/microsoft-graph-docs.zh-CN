---
title: synchronizationSecretKeyStringValuePair 资源类型
description: '代表单个机密值。 '
localization_priority: Normal
ms.openlocfilehash: 55cbd6b19ddf6c6f622ad7daddea569558e31f0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818730"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a>synchronizationSecretKeyStringValuePair 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表单个机密值。 

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|字符串| 可能的值为： `None`， `UserName`， `Password`， `SecretToken`， `AppKey`， `BaseAddress`， `ClientIdentifier`， `ClientSecret`， `SingleSignOnType`， `Sandbox`， `Url`， `Domain`， `ConsumerKey`， `ConsumerSecret`， `TokenKey`， `TokenExpiration`， `Oauth2AccessToken`， `Oauth2AccessTokenCreationTime`， `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.|
|值|字符串|机密的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

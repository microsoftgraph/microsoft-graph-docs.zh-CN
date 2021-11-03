---
title: verifiedPublisher 资源类型
description: 表示应用程序的已验证发布者。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: c65456a7dbe9b1adcb57a19a75ebf6322e84a189
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684061"
---
# <a name="verifiedpublisher-resource-type"></a>verifiedPublisher 资源类型

命名空间：microsoft.graph

表示已验证[的应用程序发布者。](application.md) 有关详细信息，请参阅验证[Publisher验证](/azure/active-directory/develop/publisher-verification-overview)。 已验证发布者使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 进行设置，并且只能使用 [unsetVerifiedPublisher 删除](../api/application-unsetverifiedpublisher.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|addedDateTime|DateTimeOffSet| 首次添加或最近更新已验证发布者的时间戳。 |
|displayName|字符串|应用发布者的合作伙伴中心帐户中的已验证发布者名称。|
|verifiedPublisherId|String| 应用发布者的合作伙伴中心帐户中经过验证的发布者的 ID。 |


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}
```


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: verifiedPublisher 资源类型
description: 表示已验证的应用程序发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: d998b8bf3e5ab4ad253e31a96794e8e531e6803e
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921897"
---
# <a name="verifiedpublisher-resource-type"></a>verifiedPublisher 资源类型

命名空间：microsoft.graph

表示已验证的 [应用程序](application.md)发布者。 有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。 已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，只能使用 [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md)删除。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|字符串|来自应用发布者的合作伙伴中心帐户的经验证的发布者名称。|
|verifiedPublisherId|字符串| 来自应用程序发布者的合作伙伴中心帐户的已验证发布者的 ID。 |
|addedDateTime|DateTimeOffSet| 首次添加或最近更新的已验证发布者时的时间戳。 |


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

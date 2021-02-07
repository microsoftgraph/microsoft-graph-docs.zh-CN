---
title: verifiedPublisher 资源类型
description: 表示应用程序的已验证发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 0c7d500a4fd032704f36953c8bf18efe6fa0f68d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129677"
---
# <a name="verifiedpublisher-resource-type"></a>verifiedPublisher 资源类型

命名空间：microsoft.graph

表示应用程序的已验证 [发布者](application.md)。 有关详细信息，请参阅 [发布者验证](/azure/active-directory/develop/publisher-verification-overview)。 已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，并且只能使用 [unsetVerifiedPublisher 删除](../api/application-unsetverifiedpublisher.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|String|应用发布者的合作伙伴中心帐户中的已验证发布者名称。|
|verifiedPublisherId|String| 应用发布者的合作伙伴中心帐户中经过验证的发布者的 ID。 |
|addedDateTime|DateTimeOffSet| 首次添加或最近更新已验证发布者的时间戳。 |


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

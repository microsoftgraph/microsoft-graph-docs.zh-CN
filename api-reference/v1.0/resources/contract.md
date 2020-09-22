---
title: 约定资源类型
description: 表示合作伙伴租户与客户租户之间的现有合作关系。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1acb1fe92884daf42b24aac0cb8bc16a2cdc6f6d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056931"
---
# <a name="contract-resource-type"></a>约定资源类型

命名空间： microsoft. graph 表示合作伙伴租户与客户租户之间的现有合作关系。

> **重要说明：** 仅存在于合作伙伴租户中。 合作伙伴租户是属于 microsoft [云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 联合或 microsoft Advisor 合作伙伴计划一部分的 microsoft 合作伙伴的 Azure AD 租户。

## <a name="methods"></a>方法

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取合同](../api/contract-get.md) | 联系 |读取特定 contract 对象的属性。 |
|[列出合同](../api/contract-list.md) | 合同集合 | 合作伙伴租户中的合同列表。 |

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|contractType|String|约定的类型。<br><br>可能的值是：<br> *SyndicationPartner* -专为此客户 resells 和管理 O365 和 Intune 的合作伙伴。 他们转售并支持其客户。<br> *BreadthPartner* -合作伙伴能够为此客户提供管理支持。 但是，不允许合作伙伴转销给客户。<br>*ResellerPartner* -合作伙伴与联合合作伙伴相似，不同之处在于合作伙伴不具有对租户的独占访问权限。 在联合案例中，客户无法购买来自 Microsoft 或其他合作伙伴的其他直接订阅。|
|customerId|Guid|此合作关系引用的客户租户的唯一标识符。 对应于客户租户的组织资源的 id 属性。 |
|defaultDomainName|String|客户租户的默认域名的副本。 如果建立与客户的合作关系，则会进行复制。 如果客户租户的默认域名发生更改，则不会自动更新该名称。|
|displayName|String|客户租户的显示名称的副本。 如果建立与客户的合作关系，则会进行复制。 如果客户租户的显示名称发生更改，则不会自动更新。|
|id|String| 合作关系的唯一标识符。 键，只读 |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


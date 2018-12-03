---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作伙伴关系。
ms.openlocfilehash: 7465a54c735b7c1e6f9d5ecb8bf79420b8de45c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048672"
---
# <a name="contract-resource-type"></a>合同资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示合作伙伴租户与客户租户的现有合作伙伴关系。

> **重要说明：** 仅存在于合作伙伴租户中。合作伙伴租户是属于 Microsoft 合作伙伴的 Azure AD 租户，其中 Microsoft 合作伙伴是 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 计划的一部分。

## <a name="methods"></a>方法

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取合同](../api/contract-get.md) | 合同 |读取特定合同对象的属性。 |
|[列出合同](../api/contract-list.md) | 合同集合 | 合同中伙伴租户中的合同列表。 |

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|contractType|String|合同的类型。<br><br>可能的值是：<br> *SyndicationPartner* - 为此客户独家转售和管理 O365 和 Intune 的合作伙伴。他们转售并为其客户提供支持。<br> *BreadthPartner* - 合作伙伴能够为此客户提供管理支持。不过，合作伙伴不得向客户进行转售。<br>*ResellerPartner* - 与联合合作伙伴类似，但是无权对租户进行独占访问。在联合的情况下，客户不能从 Microsoft 或其他合作伙伴购买其他直接订阅。|
|customerId|Guid|此合作关系引用的客户租户的唯一标识符。对应于客户租户的组织资源的 id 属性。 |
|defaultDomainName|字符串|客户租户的默认域名的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的默认域名更改，此项将不会自动更新。|
|displayName|字符串|客户租户的显示名称的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的显示名称更改，此项将不会自动更新。|
|id|字符串| 合作伙伴关系的唯一标识符。键，只读。 |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
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
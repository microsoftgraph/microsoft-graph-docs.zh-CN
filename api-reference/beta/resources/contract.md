---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作关系。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b09d773a740a82b8424a7699f959ddb38d78e1cf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444254"
---
# <a name="contract-resource-type"></a>合同资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合作伙伴租户与客户租户的现有合作关系。

> **重要提示：** 仅存在于合作伙伴租户中。 合作伙伴租户是属于属于 Microsoft 云解决方案提供商、Office 365 联合或 Microsoft Advisor 合作伙伴计划一部分的 [Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs)合作伙伴的 Azure AD 租户。

## <a name="methods"></a>Methods

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取合同](../api/contract-get.md) | 合同 |读取特定合约对象的属性。 |
|[列出合同](../api/contract-list.md) | 合同集合 | 合作伙伴租户中的合同列表。 |

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|contractType|String|合同类型。<br><br>可能的值是：<br> *SyndicationPartner* - 专门转售和管理此客户的 O365 和 Intune 的合作伙伴。 他们转售和支持其客户。<br> *BreadthPartner* - 合作伙伴能够为此客户提供管理支持。 但是，不允许合作伙伴转售给客户。<br>*ResellerPartner* - 类似于联合合作伙伴的合作伙伴，只是合作伙伴没有对租户的独占访问权限。 在联合情况下，客户无法从 Microsoft 或其他合作伙伴购买其他直接订阅。|
|customerId|Guid|此合作关系引用的客户租户的唯一标识符。 对应于客户租户的组织资源的 ID 属性。 |
|defaultDomainName|String|客户租户的默认域名的副本。 在与客户建立合作关系时，将创建副本。 如果客户租户的默认域名发生更改，将不会自动更新它。|
|displayName|String|客户租户的租户显示名称。 在与客户建立合作关系时，将创建副本。 如果客户租户的租户更改，将不会显示名称更新。|
|id|String| 合作关系的唯一标识符。 键，只读 |

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
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



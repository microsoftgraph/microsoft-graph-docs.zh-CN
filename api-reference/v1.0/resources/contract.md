---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作关系。
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4ae85bf630e4207f2647e549fa911cc1da8d769c
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854676"
---
# <a name="contract-resource-type"></a>合同资源类型

命名空间：microsoft.graph 表示合作伙伴租户与客户租户的现有合作关系。

> **重要提示：** 仅存在于合作伙伴租户中。 合作伙伴租户Azure AD属于 Microsoft 合作伙伴的租户，这些合作伙伴属于 Microsoft 云解决方案提供商、Office 365 联合或 Microsoft Advisor 合作伙伴[](https://partnercenter.microsoft.com/en-us/partner/programs)计划。

## <a name="methods"></a>Methods

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取合同](../api/contract-get.md) | 合同 |读取特定合约对象的属性。 |
|[列出合同](../api/contract-list.md) | 合同集合 | 合作伙伴租户中的合同列表。 |

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|contractType|String|合同类型。 可能的值是：、`SyndicationPartner`、`ResellerPartner``BreadthPartner`。 请参阅下表中的 [，了解](#contracttype-values)。|
|customerId|GUID|此合作关系引用的客户租户的唯一标识符。 对应于客户租户的组织资源的 id 属性。 |
|defaultDomainName|String|客户租户的默认域名的副本。 建立与客户的合作关系后，即会进行复制。 如果客户租户的默认域名发生更改，将不会自动更新它。|
|displayName|String|客户租户显示名称。 建立与客户的合作关系后，即会进行复制。 如果客户租户的租户帐户发生更改，显示名称更新。|
|id|String| 合作关系的唯一标识符。 键，只读 |

### <a name="contracttype-values"></a>contractType 值

|成员|说明|
|:---|:---|
|SyndicationPartner|专门 *转售和管理* 此客户的 O365 和 Intune 的合作伙伴。 他们转售和支持其客户。|
|BreadthPartner|合作伙伴能够为此客户提供管理支持。 但是，不允许合作伙伴转售给客户。|
|ResellerPartner|与联合合作伙伴类似的合作伙伴，只不过合作伙伴没有对租户的独占访问权限。 在联合情况下，客户无法从 Microsoft 或其他合作伙伴购买其他直接订阅。|

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
  "customerId": "GUID",
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


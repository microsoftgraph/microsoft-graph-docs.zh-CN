---
title: person 资源类型
description: 有关来自邮件、联系人和社交网络的人员的信息聚合。 用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信 (例如电子邮件和 Skype) 的人员。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 0def5d62dd941122858ffa61bf224a9ef672ad0c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344915"
---
# <a name="person-resource-type"></a>person 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

有关来自邮件、联系人和社交网络的人员的信息聚合。 用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信 (例如电子邮件和 Skype) 的人员。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **person** |获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|birthday|string|人员的生日。|
|companyName|string|人员的公司名称。|
|department|string|人员的部门。|
|displayName|string|人员的显示名称。|
|emailAddresses|[rankedEmailAddress](rankedemailaddress.md)集合|人员的电子邮件地址。|
|givenName|string|人员的名字。|
|id|string|人员的唯一标识符。只读。|
|isFavorite|boolean|如果用户已将此人员标记为常用联系人，则为 `true`。|
|mailboxType|string|由个人的电子邮件地址表示的邮箱类型。|
|officeLocation|string|人员的办公室位置。|
|personNotes|string|用户对此人员所做的自由格式备注。|
|personType|string|人员类型, 例如通讯组列表。|
|phones|[phone](phone.md) collection|人员的电话号码。|
|postalAddresses|[location](location.md) collection|人员的地址。|
|profession|string|人员的职业。|
|源|[personDataSource](persondatasource.md)集合|用户数据来自的源, 例如目录或 Outlook 联系人。|
|surname|string|人员的姓氏。|
|title|string|人员的职务。|
|userPrincipalName|string|人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。|
|websites|[website](website.md) collection|人员的网站。|
|yomiCompany|string|人员所在公司的注音日文名称。|

## <a name="relationships"></a>Relationships

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

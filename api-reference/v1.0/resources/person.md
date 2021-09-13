---
title: person 资源类型
description: 邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 33e177875c7e7724659df79d191c2fe07bc1a2a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117800"
---
# <a name="person-resource-type"></a>person 资源类型

命名空间：microsoft.graph

邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **person** |获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|birthday|String|人员的生日。|
|companyName|String|人员的公司名称。|
|department|String|人员的部门。|
|displayName|String|人员的显示名称。|
|scoredEmailAddresses|[scoredEmailAddress](scoredemailaddress.md) collection|人员的电子邮件地址。|
|givenName|String|人员的名字。|
|id|字符串|人员的唯一标识符。只读。|
|imAddress|String|用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。|
|isFavorite|Boolean|如果用户已将此人员标记为常用联系人，则为 `true`。|
|jobTitle|String|人员的职务。|
|officeLocation|String|人员的办公室位置。|
|personNotes|String|用户对此人员所做的自由格式备注。|
|personType|[personType](persontype.md) |人员类型。|
|phones|[phone](phone.md) collection|人员的电话号码。|
|postalAddresses|[location](location.md) collection|人员的地址。|
|profession|String|人员的职业。|
|surname|String|人员的姓氏。|
|userPrincipalName|字符串|人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。|
|websites|[website](website.md) collection|人员的网站。|
|yomiCompany|String|人员所在公司的注音日文名称。|

## <a name="relationships"></a>Relationships

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


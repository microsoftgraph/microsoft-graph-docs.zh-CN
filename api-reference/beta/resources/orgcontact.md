---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b7c80131cb6f8c73cd441d4c19eef17896145af8
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151438"
---
# <a name="orgcontact-resource-type"></a>orgContact 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表组织联系人。 组织联系人由组织的管理员管理，不同于个人 [联系人](contact.md)。 此外，组织联系人从本地目录或本地目录Exchange Online同步，并且为只读。

继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/orgcontact-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
| ------ | ----------- | ----------- |
| [列出组织联系人](../api/orgcontact-list.md) | [orgContact](orgcontact.md) 集合 | 列出组织联系人的属性。 |
| [获取组织联系人](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | 读取 orgContact 对象的属性和关系。 |
| [获取经理](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | 获取联系人的经理。 |
| [获取 transitiveReports](../api/orgcontact-get-transitivereports.md) | 整数 | 从 transitiveReports 导航属性获取组织联系人的可传递报告数。 |
| [List directReports](../api/orgcontact-list-directreports.md) | [directoryObject](directoryobject.md) collection | 列出联系人的直接下属。 |
| [List memberOf](../api/orgcontact-list-memberof.md) | [directoryObject](directoryobject.md) collection | 获取 memberOf 对象集合。 |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md) | String collection | 检查组成员身份。 |
| [getMemberGroups](../api/orgcontact-getmembergroups.md) | String collection | 返回指定联系人是其中成员的所有组。 |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md) | String collection | 返回联系人是其中一个成员的 directoryObjects 列表。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| -------- | ---- | ----------- |
| 地址 | [physicalOfficeAddress](physicalofficeaddress.md) 集合 | 此组织联系人的邮寄地址。 目前，联系人只能有一个物理地址。 |
| companyName | String | 此组织联系人所属的公司的名称。 |
| 部门 | String | 联系人工作部门的名称。 |
| displayName | String | 此组织联系人的显示名称。 |
| givenName | String | 此组织联系人的名字。 |
| id | String | 此组织联系人的唯一标识符。 |
| jobTitle | String | 此组织联系人的工作职务。 |
| mail | String | 联系人的 SMTP 地址，例如"jeff@contoso.onmicrosoft.com"。 |
| mailNickname | String | 电子邮件别名 (电子邮件地址的一部分预先挂起的 @ 符号) 此组织联系人。 |
| onPremisesLastSyncDateTime | DateTimeOffset | 上次从本地 AD 同步此组织联系人的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| onPremisesProvisioningErrors | [onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合 | 此组织联系人的任何同步设置错误的列表。 |
| onPremisesSyncEnabled | Boolean | 如果此对象从本地目录同步，则其为 **true;****假** 如果此对象最初从本地目录同步，但不再同步，现在在Exchange;**如果** 从未从本地目录同步此对象， (默认值) 。 |
| phones | [phone](phone.md) collection | 此组织联系人的电话列表。 电话类型可以是移动、商业和 businessFax。 集合中只能存在每种类型之一。 |
| proxyAddresses | String collection | 例如："SMTP： bob@contoso.com"、"smtp： bob@sales.contoso.com"。 需要多值属性筛选器表达式的 **any** 运算符。 支持 $filter。 |
| surname | String | 此组织联系人的姓氏。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
| ------------ | ---- | ----------- |
| directReports | [directoryObject](directoryobject.md) collection | 联系人的直接下属。  (其 manager 属性设置为此联系人的用户和联系人。) 只读。 可为 Null。 |
| manager | [directoryObject](directoryobject.md) | 作为此联系人的经理的用户或联系人。 只读。 |
| memberOf | [directoryObject](directoryobject.md) collection | 此联系人是其中一个成员的组。 只读。 可为 Null。 |
| transitiveReports | [directoryObject](directoryobject.md) collection | 联系人的可传递报告。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.orgContact"
}-->

``` json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```

---
title: orgContact 资源类型
description: 代表组织联系人
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5db56af8b2f734044331c0aab3320c6e25d49e39
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014297"
---
# <a name="orgcontact-resource-type"></a>orgContact 资源类型

命名空间：microsoft.graph

代表组织联系人。 组织联系人由组织的管理员管理，不同于个人 [联系人](contact.md)。 此外，组织联系人从本地目录或本地目录Exchange Online同步，在 Microsoft Graph。

继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/orgcontact-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。 此资源是允许传入其他属性的开放类型。

## <a name="methods"></a>Methods

| 方法                                                                  | 返回类型                                      | Description                                                                                                                 |
|:------------------------------------------------------------------------|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------|
| **组织联系人** |
| [列出组织联系人](../api/orgcontact-list.md)               | [orgContact](orgcontact.md)                      | 列出组织联系人的属性。                                                                                 |
| [获取组织联系人](../api/orgcontact-get.md)                  | [orgContact](orgcontact.md)                      | 读取组织联系人的属性和关系。                                                             |
| **组织层次结构** |
| [获取经理](../api/orgcontact-get-manager.md)                         | [directoryObject](directoryobject.md)            | 获取组织联系人的经理。                                                                                   |
| [List directReports](../api/orgcontact-list-directreports.md)           | [directoryObject](directoryobject.md) collection | 列出组织联系人的直接下属。                                                                           |
| [List memberOf](../api/orgcontact-list-memberof.md)                     | [directoryObject](directoryobject.md) 集合 | 列出组织联系人是其中一个成员的组。                                                                   |
| [列出 transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) | [directoryObject](directoryobject.md) 集合 | 列出组织联系人是其中一个成员的组，包括组织联系人嵌套在的组。 |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md)             | String collection                                | 检查组成员身份。                                                                                                 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md)                 | String collection                                | 返回指定的组织联系人是成员的所有组。                                             |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md)               | String collection                                | 返回组织联系人是其中一个成员的 directoryObjects 列表。                                               |

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#organizational-contacts-properties)。

| 属性                     | 类型                                                                     | Description                                                                                                                                                                                                                                                                                                                        |
|:-----------------------------|:-------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 地址                    | [physicalOfficeAddress](physicalofficeaddress.md) 集合             | 此组织联系人的邮寄地址。 目前，联系人只能有一个物理地址。                                                                                                                                                                                                                            |
| CompanyName                  | String                                                                   | 此组织联系人所属的公司的名称。  支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                                          |
| 部门                   | String                                                                   | 联系人工作部门的名称。  支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                                                   |
| displayName                  | String                                                                   | 此组织联系人的显示名称。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。                                                                                                                                                                                   |
| givenName                    | String                                                                   | 此组织联系人的名字。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                                                                |
| id                           | String                                                                   | 此组织联系人的唯一标识符。  支持 `$filter`（`eq`、`ne`、`not`、`in`）。                                                                                                                                                                                                                                  |
| jobTitle                     | String                                                                   | 此组织联系人的工作职务。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                                                                 |
| mail                         | String                                                                   | 联系人的 SMTP 地址，例如"jeff@contoso.onmicrosoft.com"。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                             |
| mailNickname                 | String                                                                   | 电子邮件别名 (电子邮件地址的一部分预先挂起的 @ 符号) 此组织联系人。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                           |
| onPremisesLastSyncDateTime   | DateTimeOffset                                                           | 上次从本地 AD 同步此组织联系人的日期和时间。 此日期和时间信息使用 ISO 8601 格式，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`）。                             |
| onPremisesProvisioningErrors | [onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合 | 此组织联系人的任何同步设置错误的列表。 支持 `$filter`（`eq`、`not`）。                                                                                                                                                                                                                 |
| onPremisesSyncEnabled        | Boolean                                                                  | `true`如果此对象从本地目录同步;如果此对象最初从本地目录同步，但不再同步，现在在 Exchange 中主控;如果此对象从未从本地目录同步过 (`false` `null` 默认) 。 <br/> <br/> 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。 |
| phones                       | [phone](phone.md) collection                                             | 此组织联系人的电话列表。 电话类型可以是移动、商业和 businessFax。 集合中只能存在每种类型中的一种。                                                                                                                                                                 |
| proxyAddresses               | String collection                                                        | 例如："SMTP： bob@contoso.com"、"smtp： bob@sales.contoso.com"。 需要多值属性筛选器表达式的 **any** 运算符。 支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。                                                                                                               |
| surname                      | String                                                                   | 此组织联系人的姓氏。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。                                                                                                                                                                                                                 |

## <a name="relationships"></a>关系

| 关系       | 类型                                             | Description                                                                                                                                            |
|:-------------------|:-------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|
| directReports      | [directoryObject](directoryobject.md) collection | 联系人的直接下属。  (其经理属性设置为此联系人的用户和联系人。) 只读。 可为 NULL。 支持 `$expand`。 |
| manager            | [directoryObject](directoryobject.md)            | 作为此联系人的经理的用户或联系人。 只读。 支持 `$expand`。                                                                     |
| memberOf           | [directoryObject](directoryobject.md) 集合 | 此联系人是其中一个成员的组。 只读。 可为 NULL。 支持 `$expand`。                                                                      |
| transitiveMemberOf | [directoryObject](directoryobject.md) 集合 | 此联系人是其中一个成员的组，包括该联系人嵌套在的组。 只读。 可为 Null。                                       |

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
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


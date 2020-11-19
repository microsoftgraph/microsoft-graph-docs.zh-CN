---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ccd36e9d04a1404bb972694fdb9c2b0d8a5ccc3
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352367"
---
# <a name="orgcontact-resource-type"></a>orgContact 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个组织联系人。 组织联系人由组织的管理员管理，不同于 [个人联系人](contact.md)。 此外，组织联系人既可以从本地目录同步，也可以从 Exchange Online 同步，也可以是只读的。

继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/orgcontact-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | Description |
| ------ | ----------- | ----------- |
| [列出组织联系人](../api/orgcontact-list.md) | [orgContact](orgcontact.md) 集合 | 列出组织联系人的属性。 |
| [获取组织联系人](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | 读取 orgContact 对象的属性和关系。 |
| [获取管理器](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | 获取联系人的经理。 |
| [List directReports](../api/orgcontact-list-directreports.md) | [directoryObject](directoryobject.md) collection | 列出联系人的直接下属。 |
| [List memberOf](../api/orgcontact-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 获取 memberOf 对象集合。 |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md) | String 集合 | 检查组成员身份。 |
| [getMemberGroups](../api/orgcontact-getmembergroups.md) | String 集合 | 返回指定的联系人所属的所有组。 |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md) | String 集合 | 返回联系人所属的 directoryObjects 的列表。 |

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
| -------- | ---- | ----------- |
| 地址 | [physicalOfficeAddress](physicalofficeaddress.md) 集合 | 此组织联系人的邮政地址。 目前，一个联系人只能有一个实际地址。 |
| companyName | String | 此组织联系人所属的公司的名称。 |
| department | String | 联系人工作所在的部门的名称。 |
| displayName | 字符串 | 此组织联系人的显示名称。 |
| givenName | 字符串 | 此组织联系人的名字。 |
| id | 字符串 | 此组织联系人的唯一标识符。 |
| jobTitle | String | 此组织联系人的职务。 |
| mail | String | 联系人的 SMTP 地址，例如，"jeff@contoso.onmicrosoft.com"。 |
| mailNickname | String | 电子邮件别名 (电子邮件地址的一部分预挂起此组织联系人的 @ 符号) 。 |
| onPremisesLastSyncDateTime | DateTimeOffset | 上次从本地 AD 同步此组织联系人的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| onPremisesProvisioningErrors | [onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合 | 此组织联系人的任何同步设置错误列表。 |
| onPremisesSyncEnabled | Boolean | 如果此对象从本地目录同步，**则为 true** ; 否则为 false。**假** 如果此对象最初是从本地目录同步，但不再同步，并且现在在 Exchange 中的 mastered;如果从未从本地目录同步此对象，则 **为 null** (默认) 。 |
| phones | [phone](phone.md) collection | 此组织联系人的电话列表。 电话类型可以是移动、商业和 businessFax。 集合中仅有一种类型可以存在。 |
| proxyAddresses | String 集合 | 例如： "SMTP： bob@contoso.com"、"SMTP： bob@sales.contoso.com"。 需要多值属性筛选器表达式的 **any** 运算符。 支持 $filter。 |
| surname | 字符串 | 此组织联系人的姓氏。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | Description |
| ------------ | ---- | ----------- |
| directReports | [directoryObject](directoryobject.md) collection | 联系人的直接下属。  (其 "经理" 属性设置为 "联系人" 的用户和联系人。 ) 只读。 可为 Null。 |
| manager | [directoryObject](directoryobject.md) | 作为此联系人的经理的用户或联系人。 只读。 |
| memberOf | [directoryObject](directoryobject.md) 集合 | 此联系人所属的组。 只读。 可为 Null。 |

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

---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01f606e8fb1f6ae51608853eed3bc39e0ec124df
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643529"
---
# <a name="orgcontact-resource-type"></a>orgContact 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 orgContact](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |读取属性和 orgContact 对象的关系。|
|[获取管理器](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| 获取联系人的经理。|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| 列出该联系人的直接下属。|
|[List memberOf](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md) collection| 获取 memberOf 对象集合。|
|[删除](../api/orgcontact-delete.md) | 无 |删除 orgContact 对象。 |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection| 检查组成员身份。 |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String collection| 返回指定的联系人所在的所有组。 |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection| 返回的 directoryObjects 联系人所在的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| addresses                    | [physicalOfficeAddress](physicalofficeaddress.md)            | 此组织联系人的的邮政地址。 现在联系人只能有一个物理地址。 |
| companyName                  | String                                                    | 此组织联系人属于公司的名称。                                                                                                                                                                                                                                                                                                                 |
| department                   | String                                                     | 联系人适用于该部门的名称。                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | 此组织联系人的显示名称。                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | 此组织联系人的名字。                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | 此组织联系人的的唯一标识符。                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | String collection                          | 为此组织联系人的 IM 地址列表。 现在联系人只能有一个 SIP 地址。                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | 此组织联系人的职务。                                                                                                                                                                                                                                                                                                                                      |
|mail|String| 该联系人，例如，"jeff@contoso.onmicrosoft.com"的 SMTP 地址。 |
| mailNickname                 | String                                                     | 电子邮件别名 (预挂起的电子邮件地址部分 @ 符号) 为此组织联系人。                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | 日期和时间此组织联系人上次同步从内部部署 AD。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，在 2014 年 1 月 1 日午夜 UTC 如下所示:"2014年-01-01T00:00:00Z。   |
| onPremisesProvisioningErrors |[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合       | 设置为此组织联系人错误任何同步的列表。                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Boolean|**true**如果此对象同步从内部部署目录;**false**如果此对象最初从内部部署目录同步，但不再同步并立即掌握 Exchange;**null**如果此对象包含从不已同步从内部部署目录 （默认值）。|
| phones                       | [phone](phone.md) collection                            | 为此组织联系人的电话的列表。 电话类型可以是移动、 业务和商务传真。 每种类型的唯一一个以往任何时候都可以存在集合中。                                                                                                                       |
| proxyAddresses               | String collection                                         | 例如: ["SMTP: bob@contoso.com"，"smtp: bob@sales.contoso.com"]。 多值属性筛选器表达式需要 **any** 运算符。 支持\$筛选器。                                                                                                                                                                               |
| surname                      | String                                                     | 此组织联系人的的姓。                          |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| 联系人的直接下属。 （用户和其管理器属性设置为此联系人的联系人。） 只读的。 可为 Null。|
|manager|[directoryObject](directoryobject.md)| 用户或此联系人的管理器的联系人。 只读。|
|memberOf|[directoryObject](directoryobject.md) collection| 此联系人所在的组。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/orgcontact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

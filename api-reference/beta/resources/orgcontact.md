---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046986"
---
# <a name="orgcontact-resource-type"></a>orgContact 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|city|字符串| 联系人所在的市/县。 |
|country|字符串| 联系人所在的国家/地区。 |
|department|字符串| 联系人适用于该部门的名称。 |
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。|
|displayName|字符串| 该联系人的显示名称。 |
|givenName|字符串| 联系人的给定姓名 （名字）。 |
|jobTitle|字符串| 联系人的职务。 |
|onPremisesLastSyncDateTime|DateTimeOffset|指示的上次与内部部署目录同步对象的频率。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)集合| 设置过程中使用 Microsoft 同步产品时错误。 |
|mail|字符串| 该联系人，例如，"jeff@contoso.onmicrosoft.com"的 SMTP 地址。 |
|mailNickname|字符串| 邮件联系人的别名。 |
|mobilePhone|String| 联系人的主要移动电话号码。 |
|id|字符串| 该联系人的唯一标识符。 只读。|
|officeLocation|String| 中的业务联系人的位置的办公室位置。 |
|postalCode|字符串| 联系人的邮政地址的邮政编码。 特定于该联系人的国家/地区的邮政编码。 在美国，此属性包含邮政编码。 |
|proxyAddresses|String collection| 例如： `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**运算符，则需要为多值属性的筛选器表达式。 只读。 不可为 null。 支持 $filter。 |
|状态|字符串| 州或省中联系人的地址。 |
|streetAddress|String| 联系人的位置的业务街道地址。 |
|surname|字符串| （家人名称或姓氏） 的联系人的姓。 |
|businessPhones|String| 联系人的位置的业务主要电话号码。 |

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| 联系人的直接下属。 （用户和其管理器属性设置为此联系人的联系人。） 只读的。 可为 Null。|
|manager|[directoryObject](directoryobject.md)| 用户或此联系人的管理器的联系人。 只读。|
|memberOf|[directoryObject](directoryobject.md) 集合| 此联系人所在的组。 只读。 可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 orgContact](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |读取属性和 orgContact 对象的关系。|
|[获取管理器](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| 获取联系人的经理。|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| 列出该联系人的直接下属。|
|[List memberOf](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 获取 memberOf 对象集合。|
|[删除](../api/orgcontact-delete.md) | 无 |删除 orgContact 对象。 |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection| 检查组成员身份。 |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String collection| 返回指定的联系人所在的所有组。 |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection| 返回的 directoryObjects 联系人所在的列表。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
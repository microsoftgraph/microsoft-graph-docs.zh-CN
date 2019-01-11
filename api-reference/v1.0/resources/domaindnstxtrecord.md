---
title: domainDnsTxtRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 TXT 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 81b55bafc07dda0900c57505805c5ac1ed2ebf51
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890025"
---
# <a name="domaindnstxtrecord-resource-type"></a>domainDnsTxtRecord 资源类型

表示已添加到租户中特定域的 DNS 区域文件的 TXT 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

## <a name="methods"></a>方法
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 分配给此实体的唯一标识符。不可为 NULL，只读。 |
|isOptional|Boolean| 如果为 false，则客户必须在 DNS 主机上配置 TXT 记录才能使 Microsoft Online Services 在域中正常运行。 |
|label|String| 配置 DNS 主机上的 TXT 记录的*名称*属性时使用的值。|
|recordType|String| DNS 记录类型。此值始终是 *Txt*。Key |
|supportedService|String| Microsoft Online Service 或与该 TXT 记录存在依赖关系的功能。</br></br>可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune* |
|text|String| 配置 DNS 主机上的*文本*属性时使用的值。 |
|ttl|Int32| 配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

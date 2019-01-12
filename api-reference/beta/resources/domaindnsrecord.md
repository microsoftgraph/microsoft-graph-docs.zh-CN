---
title: domainDnsRecord 资源类型
description: 对于租户中的每个域，您可能需要先域可由 Microsoft Online Services 将 DNS 记录添加到域的 DNS 区域文件。 **DomainDnsRecord**实体用于显示此类的 DNS 记录。 DomainDnsCnameRecord、 DomainDnsMxRecord、 DomainDnsSrvRecord 和 DomainDnsSrvRecord 实体的基准实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5c760ba9a2100bbefd0353c2c02019e7a04354b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912958"
---
# <a name="domaindnsrecord-resource-type"></a>domainDnsRecord 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

对于租户中的每个域，可能需要先将 DNS 记录添加到相应域的 DNS 区域文件，然后 Microsoft Online Services 才能使用该域。**DomainDnsRecord** 实体用于显示这些 DNS 记录。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和 [DomainDnsSrvRecord](domaindnssrvrecord.md) 实体的基本实体。

## <a name="methods"></a>方法
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 分配给此实体的唯一标识符。不可为 NULL，只读。|
|isOptional|Boolean| 如果为 false，则客户必须在 DNS 主机上配置此记录才能使 Microsoft Online Services 在域中正常运行。 |
|label|String| 配置 DNS 主机上的 DNS 记录的名称时使用的值。 |
|recordType|String| 指示此实体表示的 DNS 记录类型。</br></br>值可以是下列值之一：*CName*、*Mx*、*Srv*、*Txt*</br></br>Key |
|supportedService|String| Microsoft Online Service 或与该 DNS 记录存在依赖关系的功能。</br></br>可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*|
|ttl|Int32| 配置 DNS 主机上的 DNS 记录的生存时间 (ttl) 属性时使用的值。不可为 null |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

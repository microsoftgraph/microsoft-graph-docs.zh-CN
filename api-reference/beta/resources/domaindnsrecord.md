---
title: domainDnsRecord 资源类型
description: domainDnsRecord 实体用于呈现 DNS 记录。
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 327a07fcbca5c9c02bca90e46ceff9454c3267f3
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246557"
---
# <a name="domaindnsrecord-resource-type"></a>domainDnsRecord 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对于租户中的每个 [域](domain.md) ，可能需要将 DNS 记录 () 添加到域的 DNS 区域文件，然后 Microsoft Online Services 才能使用该域。 **domainDnsRecord** 实体用于呈现此类 DNS 记录。 此资源类型是以下资源的基础实体：
+ [domainDnsCnameRecord](domaindnscnamerecord.md)
+ [domainDnsMxRecord](domaindnsmxrecord.md)
+ [domainDnsSrvRecord](domaindnssrvrecord.md)
+ [domainDnsTxtRecord](domaindnstxtrecord.md)
+ [domainDnsUnavailableRecord](domaindnsunavailablerecord.md)

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 分配给此实体的唯一标识符。 不可为 null，只读。|
|isOptional|Boolean| 如果为 false，则必须由 DNS 主机的客户配置此记录，以便 Microsoft Online Services 在域中正常运行。 |
|标签|String| 在 DNS 主机上配置 DNS 记录的名称时使用的值。 |
|recordType|String| 指示此实体表示的 DNS 记录类型。</br></br>该值可以是下列值之一： `CName`， ， `Mx``Srv`， . `Txt` |
|supportedService|String| 依赖于此 DNS 记录的 Microsoft Online 服务或功能。</br></br>可以是下列值之一：`null`、`Email`、、`Sharepoint`、`OfficeCommunicationsOnline``EmailInternalRelayOnly`、`SharePointDefaultDomain`、`FullRedelegation`、`SharePointPublic`、`OrgIdAuthentication`、`Yammer`、 `Intune`|
|Ttl|Int32| 在 DNS 主机上配置 DNS 记录的生存时间 (ttl) 属性时使用的值。 不可为空。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



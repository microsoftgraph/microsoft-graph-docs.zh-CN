---
title: domainDnsRecord 资源类型
description: DomainDnsRecord 实体用于显示 DNS 记录。
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fdd8dd884b19803aede0109a9c5c95bb3abe8585
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123794"
---
# <a name="domaindnsrecord-resource-type"></a>domainDnsRecord 资源类型

命名空间：microsoft.graph

对于租户中的每个域，可能需要将 dns 记录 () 添加到域的 DNS 区域文件中，然后该域才能由 Microsoft Online Services。 **DomainDnsRecord** 实体用于显示此类 DNS 记录。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和[DomainDnsTxtRecord](domaindnstxtrecord.md)实体的基实体。 [](domaindnscnamerecord.md) [](domaindnsmxrecord.md) [](domaindnssrvrecord.md)

## <a name="methods"></a>方法
不支持直接查询此资源。 请参阅 [域主题](domain.md) ，了解如何查询域服务记录。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 分配给此实体的唯一标识符。 不可为空，只读。|
|isOptional|Boolean| 如果为 false，则客户必须在 DNS 主机上配置此记录Microsoft Online Services该域正常运行。 |
|标签|String| 在 DNS 主机上配置 DNS 记录的名称时所使用的值。 |
|recordType|String| 指示此实体表示的 DNS 记录类型。</br></br>值可以是以下值之一：CName、Mx、Srv、Txt    </br></br>键 |
|supportedService|String| 依赖此 DNS 记录的 Microsoft Online 服务或功能。</br></br>可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           |
|ttl|Int32| 在 DNS 主机上配置 DNS 记录 (ttl) 时要使用的值。 不可为 null |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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


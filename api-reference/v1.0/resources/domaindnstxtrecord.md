---
title: domainDnsTxtRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件的 TXT 记录。
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4820490b65d5186267c3e25318638bb9d4739596
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123746"
---
# <a name="domaindnstxtrecord-resource-type"></a>domainDnsTxtRecord 资源类型

命名空间：microsoft.graph

表示添加到租户中特定域的 DNS 区域文件的 TXT 记录。 继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

## <a name="methods"></a>方法
不支持直接查询此资源。 请参阅 [域主题](domain.md) ，了解如何查询域服务记录。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 分配给此实体的唯一标识符。 不可为空，只读。 |
|isOptional|Boolean| 如果为 false，则客户必须在 DNS 主机上配置 TXT 记录，Microsoft Online Services该域正常运行。 |
|标签|String| 在 DNS 主机上配置TXT 记录的名称属性时要使用的值。|
|recordType|String| DNS 记录的类型。 该值始终为 *Txt*。 键 |
|supportedService|String| 依赖此 TXT 记录的 Microsoft Online Service 或功能。</br></br>可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune            |
|text|String| 在 DNS 主机上配置 *文本* 属性时所使用的值。 |
|ttl|Int32| 在 DNS 主机上配置 MX 记录的 ttl (*ttl*) 时要使用的值。 不可为 null |

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


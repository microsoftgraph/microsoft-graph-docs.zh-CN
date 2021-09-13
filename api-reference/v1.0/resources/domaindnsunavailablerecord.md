---
title: domainDnsUnavailableRecord 资源类型
description: 指示无法生成 serviceConfigurationRecords。
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: cda989c9033818efe7f750467783bb5f2ce517a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123760"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord 资源类型

命名空间：microsoft.graph

查询 [Domain](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可以返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md)实体。 [](domaindnscnamerecord.md) [](domaindnsmxrecord.md) [](domaindnssrvrecord.md) 这些实体指示必须先将哪些 DNS 记录添加到域的区域文件，然后该域才能由 Microsoft Online Services。 如果无法生成此类实体，则改为返回 DomainDnsUnavailableRecord Entity。 继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

## <a name="methods"></a>方法
不支持直接查询此资源。 请参阅 [域主题](domain.md) ，了解如何查询域服务记录。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|提供返回 **DomainDnsUnavailableRecord** 实体的原因。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


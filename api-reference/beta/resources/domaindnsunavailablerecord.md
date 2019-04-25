---
title: domainDnsUnavailableRecord 资源类型
description: 当您查询 Domain 实体的导航属性**serviceConfigurationRecords**时, 您可能会返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须添加到域的区域文件中的 DNS 记录, 在 Microsoft Online Services 可使用域之前。 如果不能生成此类实体, 则改为返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe3c1eeae7ae3ddb634a3c120332dd8d8996f41c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535030"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord 资源类型

当您查询[Domain](domain.md)实体的导航属性**serviceConfigurationRecords**时, 您可能会收到一个或多个[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和/或[DomainDnsTxtRecord](domaindnstxtrecord.md)实体。 这些实体指示您必须添加到域的区域文件中的 DNS 记录, 在 Microsoft Online Services 可使用域之前。 如果不能生成此类实体, 则改为返回 DomainDnsUnavailableRecord 实体。 继承自[DomainDnsRecord](domaindnsrecord.md)实体。

## <a name="methods"></a>方法
不支持直接向此资源进行查询。 有关如何查询域服务记录的信息, 请参阅[域](domain.md)主题。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|提供**DomainDnsUnavailableRecord**实体返回的原因。 |

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
